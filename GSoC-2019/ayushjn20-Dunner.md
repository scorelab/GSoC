# Dunner
> A docker based task runner tool.

## Student Info
- __Name:__ Ayush Jain
- __Email ID:__ [ayushjain20n@gmail.com](mailto:ayushjain20n@gmail.com)
- __GitHub:__ [@ayushjn20](https://github.com/ayushjn20)
- __LinkedIn__:[@ayushjn20](https://www.linkedin.com/in/ayushjn20) 
- __Resume:__ [[pdf](https://drive.google.com/file/d/1oTeMR6acD8vrEfZfaVSuFaMq5YT3cuCS/view)]

### Project Abstract
Dunner is a container based task runner tool built in Golang using Docker’s client library. A user
can define multiple tasks, each task with some sequential steps which run on separate
containers. Salient features are as follows.

- Easy to write YAML task file, validate the file before execution
- A test run mode, viz., Dry run
- Passing arguments through cli
- Exporting environment variables from the host or .env file
- Mounting external directories as bind volumes
- Concurrent execution of tasks by choice
- Use one task as a step in another step
- Define directory mounts and environment variables common to a task or step

Docker has proven to be a great utility tool when talked about the DevOps existing in the
current trend of software development. It’s open source, easy-to-use, reliable and reduces
system dependencies on a very large scale. The motivation in choosing Docker as the backbone
of a task-runner is that no dependencies are being installed on the host directly, and no
execution process interacts with host at core-level. This increases system security such that
whatever be the process, it gets executed in the container itself. Therefore, if the process is
meant to harm the system, only that specific container will get affected, not the host.



## Useful Links

#### GSoC Project Page: [[link](https://summerofcode.withgoogle.com/projects/#5461263713304576)]

#### GSoC Project Proposal: [[pdf](https://drive.google.com/file/d/1Rf-YIoCQT2e4bB9Agg8ha5wQQZPm98Wd/view)]

#### GitHub Organization: [LeopardsLab](https://github.com/leopardslab)

#### GitHub Organization Repo: [dunner](https://github.com/leopardslab/dunner)

#### GitHub Personal Repo: [dunner](https://github.com/ayushjn20/dunner)


## Commits during GSoC 2018
Commits related to Dunner are spread across various repositories of LeopardsLab, major ones are below:

* [Dunner](https://github.com/leopardslab/dunner/commits/develop?author=ayushjn20)
* [Dunner Wiki](https://github.com/ayushjn20/dunner-wiki/commits?author=ayushjn20)
* [installer.to](https://github.com/leopardslab/installer.to/commits?author=ayushjn20)
* [Dunner Website](https://github.com/leopardslab/dunner-website/commits?author=ayushjn20)

### Work Summary
#### [Dunner](https://github.com/leopardslab/dunner)
- Worked on generating different kinds of installation packages compatible with different OSs and architectures. GoReleaser was primarily used to generate all the packages. This was then configured with Travis-CI for auto-deployment. Following types of packages were generated
-- rpm
-- deb
-- binary tar balls for different architectures
-- brew package
-- apt package
-- snap package
-- exe (for windows)

- Added dynamic validation of the dunner task file. There is a separate sub-command for validating, as well as the file is validated before actual execution.

- Add support for execution of multiple commands within the same container as one complete step. This means that if someone needs to use the effect of one command in the next command, he/she can define that in the same step.

- Implemented a dry run mode that enables users to check more than config validation without actually executing the commands.

- Added proper inline comments ( with examples at appropriate places) to help anyone who wants to understand the code, or use dunner as a library. This also populated content in the GoDoc reference of dunner.

- Added the ability to check for locally built images without actually taking from Docker Hub always.

- Added enough unit tests to improve the code coverage. At the time writing, we have achieved around ~75% coverage as per the report by Codecov.

- Implemented inline loading message to make it clear that dunner is busy doing some process.

- Restructured the dunner task file parsing to incorporate of setting configs like environment variables and directory mounts common to all the tasks and/or common to all the steps of a particular task.
 
- Added pre-commit git hook.

#### [Dunner Wiki](https://github.com/leopardslab/dunner/wiki)
Worked extensively on [User Guide](https://github.com/leopardslab/Dunner/wiki/User-Guide) which has detailed documentation regarding how a user can exploit various features of dunner. 

#### [Dunner Website](https://github.com/leopardslab/dunner-website)
Used Gatsby framework to make a nice website. The highlight of my work was rendering the wiki (written in Markdown) into Gatsby pages for showing this wiki as documentation on the website. It was hosted using Netlify. 

#### [Installation Script](https://github.com/leopardslab/installer.to/pull/21)
The installation script can dynamically detect proper installation method/package on the basis of OS and architecture present on the host machine. This script was designed in such a way that it may work on almost all the known platforms which can support docker and golang.

#### [AUR Package](https://aur.archlinux.org/packages/dunner)
Worked on building this package repository for installation on Arch linux, something that GoReleaser does not provide at the time of writing.


## What is left to do

- **Dunner Daemon**: The aim of having a daemon service for dunner is to allow the usage of dunner through other programming languages as well. The idea is to create a http listener that can listen to RESTful APIs for creating, updating, deleting, and executing tasks through dunner. 

- **Resource Usage Profiling**: A task runner will always look incomplete if it is not able to give the the extent of resources used during the execution of the task. The useful information can be time elapsed, CPU usage graph, memory usage graph, etc. 

-  **Global logging**: A global host-level logging onto file-system for permanent trace on when and what dunner has performed so far. 

### References
- [Dunner](https://github.com/leopardslab/dunner)
- [Dunner Wiki](https://github.com/leopardslab/dunner/wiki)
- [Dunner Website](https://dunner.io)
- [Dunner GoDoc](https://godoc.org/github.com/leopardslab/dunner)
- [Installation Script](https://github.com/leopardslab/installer.to/blob/master/installers/dunner/installer.sh)
- [AUR Package](https://aur.archlinux.org/packages/dunner)
