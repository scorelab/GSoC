# Automated deployments and testing for installer.to

## Student Info

* Name - Heshan Geasman
* Email - HeshDude@gmail.com
* GitHub profile - https://github.com/Heshdude
* Twitter - [@Heshdude](https://twitter.com/Heshdude)

### Project Abstract

installer.to is a repository of installation scripts where anyone can pull an installer script simply with `cURL`

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4739629707689984)

### [GSoC Project Proposal](https://docs.google.com/document/d/1ETznT5WCEsJytbA19JxpIMqPqjGTpncK_8RFCgQdszI/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/leopardslab/installer.to)

### [GitHub Personal Repo](https://github.com/Heshdude/installer.to)

### [Commits during GSoC 2019](https://github.com/leopardslab/installer.to/commits?author=Heshdude)

### [GSoC Blog](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-10-75f7c4f5b1b3)

### Work Summary

I implemented the Continuous Integration and Continuous Delivery for installer.to and 
introduced a new way of defining the installation steps, 
where the installations scripts are then generated from this in the Continuous Delivery flow.
Finally a way to users to hint about the package manager they are interested in getting the installation steps.


### What Covered

#### 1. Installation script generator
Here contributors can define the installation steps in a TOML file called `installer.toml` in simple format as below,
```
name = "Git"
shortname = "git"
description = "Git SVM"
issue = "https://github.com/leopardslab/installer.to/issues/1"

[apt]
sh = """
@sudo apt-get update
@sudo apt-get install git
"""

[yum]
sh = """
@sudo yum install git
"""

[pacman]
sh = """
pacman -Sy git
"""
```

Generator can read this file and generate the `installer.sh` using the installation steps for each package manager.
The reason for this setup is, earlier, the installation scripts had different methods of sniffing the available package managers,
and the installer scripts looks complex for new contributors to come contribute to the installer scripts repo.
However, now the package manager sniffing code snipets are added by the generator and is consistent in all the installer script.
Furthermore, because the `installer.toml` looks very clean and simple, anyone can add installation steps of their favorite tools.

Generator generates a minified version of the `installer.sh` as `installer.min.sh` using a shell script minifier. Also,
it creates package manager specific installation scripts and their monified versions like, 

1. `installer.apt.sh`
2. `installer.apt.min.sh`
3. `installer.yum.sh`
4. `installer.yum.min.sh`

for all the package managers defined in the `installer.toml`. The reason for this is explained in #

Generator also injects the code snippets to sniff if the user is `root` and if the system has `sudo`. 
Contributors of the installer script only has to define the places where they need `sudo` permissions with `@sudo` tag like,
``` 
[yum]
sh = """
@sudo yum install git
```

This way, if the user is not `root` and system has `sudo` this command will become `sudo yum install git`.
If the system is running as `root`, like inside a Docker container, this will be `yum install git` only.
This will make sure the installation scripts does not break with `sudo` commands appearing here and there.
Best thing is, people who contribute with creating installation scripts does not have to worry about any of these,
they simply have to put `@sudo` where they want `sudo` command to appear. Because the `installer.toml` file is simple and clean, 
it is easy for the maintainers to spot these kinda places where `sudo` is used while reviewing PRs and correct them otherwise.

I also introduced a logger into to the Generator, where if any proper log message is needs to be put, 
it can be done simply as below,
``` 
@info "Installing hello"
@warn "This is only a demo installation"
@error "Did not install hello"
```
`@log` and `@info` are info logs, `@warn` and `@error` are warning and error logs respectively. 
Logs are printed with proper timestamps and nice intuitive colors, like somewhat below, but with colours.
```
[2020.08.23-01:05:06+0530] INFO Installing hello 
[2020.08.23-01:05:06+0530] WARN This is only a demo installation 
[2020.08.23-01:05:06+0530] ERROR Did not install hello
```

Generator also updates the supported set of tools and their suported package managers in table in the `README.md` of the repo.
This generates the table with proper markdown syntax for tables. Then it updates the `installers.toml` file, 
which will be the central data source of the project, which includes all the tools and their supported package managers.


#### 2. Continuous Integration and Continuous Deployment
I implemented both CI and CD for installer.to project with GitHub Actions. Whenever a Pull Request is created to GitHub,
the installer scripts are generated only for the changed tools and tests are run for this changed tool only. 
This is to avoid taking too much time for a PR check as generating installer scripts for all the tools and running tests take time.

I built the test containers for running testing for each package manager, which has only that package manager, 'ShellSpec',
the testing framework and `expect` a tool to manipulate interactive shell scripts. 
Whenever there is change to the Dockerfiles, the GitHub Action will build the Docker images and push to the GitHub Packages.
Anyone can use these Docker images pulling from GitHub packages.
```
docker pull docker.pkg.github.com/leopardslab/installer.to/shellspec:apt
docker pull docker.pkg.github.com/leopardslab/installer.to/shellspec:yum
docker pull docker.pkg.github.com/leopardslab/installer.to/shellspec:dnf
```

When a Pull Request of an `installer.toml` is merged to the `master` branch, the Continuous Deployment flow will kick in, 
with GitHub Actions, and commit the generated/updated installer scripts, `README.md` and `installers.toml` files and
create a new PR with proper title, description mentioning the PR this PR is related to and proper labels. 
Project maintainers are notified about this new PR in the Gitter channel with links to quick navigation to both PRs.
Then they can review the generated content and merge to master. With this, anyone who likes to add a new installer for a tool,
has only has to do is create a `installer.toml`  file and create a PR. The rest of the things are all automated and done.

After generating the new installer scripts, their minified versions, etc the Continuous Deployment flow then publish these
files to the Google Cloud Storage bucket which all the installer scripts are stored. 
Finally it will update the Firebase functions, etc to update the firebase function changes if any.

#### 3. Package-manager hints in cURL queries
I also changed the Firebase function to take hints from `curl` URL's query params, like `with` and `min`.
For example, if a user send the cURL request like follows and pipe it to bash
```
curl https://installer.to/git?with=yum | bash
```

then what will be downloaded is an installer script specific to yum and other package-manager related commands will not be there. 
This makes the installers very small and downloading fast.
In addition to to the package-manager dependent flags, I also added minifying flags.
If a user sends a cURL request like follows and pipe it to bash,

``` 
curl https://installer.to/git?min=yes | bash
```
then what will be downloaded is a minified script which is smaller than the usual installer scripts. 
The best part is users can combine these two flags together.
``` 
curl https://installer.to/git?with=apt&min=yes | bash
```
When users cURL like above, they will only get the package-manager dependent installer script and it will be a minified script.

#### 5. LogDude Bash logging micro framework
While working with installer.to project, I wrote some interesting code part for a logger which shows datetime, log level, etc.
I first took out these codes and created as a personal project but then my mentors suggested it can be absorbed into LeopardsLab.
Now it is under LeopardsLab organisation as [log-dude](https://github.com/leopardslab/log-dude) 

#### 6. GatsbyJS site base 
Even though this was not in my original plan, my mentors suggested me work on this in the background as this might come handy.
I tried using the Gatsby with Apollo Docs theme and I could configure them to a simple site but could not do a lot there. 

#### 7. Created TOML files for existing installers
As now I have introduced this new `installer.toml` method, I added the `installer.toml`s to all the existing tools, except few.
These can be referred by the new contributors to get an idea on how to add new `installer.toml`s for different flavours.

### What left

- Adding testing for existing installers, as this need some more standardizing as per mentors and got deprioritized.
- Complete the GatsbyJS site ( was not in the original plan )

### Blog posts
I wrote blog posts every week except few and below are the URLs of each of the blog posts! 
1. [Working on installer.to with SCoRe Lab for GSoC 2020](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-a6c919a80ab9)
2. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 1](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-1-c89dded9a95b)
3. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 2](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-2-f9d662d7a48b)
4. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 3](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-3-824408cb5975)
5. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 4](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-4-cdf6a3ac9ea1)
6. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 5](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-5-7cb6fe292e42)
7. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 6](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-6-744ba388c9ee)
8. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 7](https://medium.com/scorelab/my-previous-medium-article-got-published-under-score-as-https-medium-com-scorelab-working-on-insta-e57972ed7bcc)
9. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 8](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-8-a09853e1c8d)
10. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 9](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-9-113c8c8708f4)
11. [Working on installer.to with SCoRe Lab for GSoC 2020: Week 10](https://medium.com/scorelab/working-on-installer-to-with-score-lab-for-gsoc-2020-week-10-75f7c4f5b1b3)
