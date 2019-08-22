# Bassa - Making Installation of Bassa and Containerize in a Better Way

## Student Info
  * Name - Mehant Kammakomati
  * Email - kmehant@gmail.com / kmehant@scorelab.org
  * University - National Institute of Technology, Andhra Pradesh
  * GitHub profile - https://github.com/kmehant
  * LinkedIn profile - https://www.linkedin.com/in/mehant-kammakomati-1a0b41170/

### Project Abstract
Bassa is an automated download queue for communities. It is an n-tier application which needs extra layers of code to make it ready for production use. Bassa has been completely containerized using docker and with docker-compose integration it made setting up and usage for developers 90% easier than before. Further these containers can be deployed over a Kubernetes cluster giving a powerful orchestration capability. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6393245309861888)

### [GSoC Project Proposal](https://drive.google.com/file/d/1kG25acRkI59siPG-TK9Fq86HIQgJpTzE/view?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab)

### [GitHub Personal Repo](https://github.com/kmehant/bassa)

### [Commits during GSoC 2018](https://github.com/scorelab/Bassa/pulls?utf8=%E2%9C%93&q=label%3AGSoC-2019+author%3Akmehant+is%3Apr+)

### [Project Demo Video](https://drive.google.com/file/d/1WAQH0W-Tr2IyDxfazr5Q4KHnJkphiXWt/view?usp=sharing)

### [Project Wiki](https://github.com/scorelab/Bassa/wiki)

### [GSoC Blog](https://gist.github.com/kmehant/bf3dfd3bcf07a611d7881c277f9fcc3b)


### Work Summary
Made installation of Bassa 90% easier for developers by implementing a generic dependency installation shell script, dockerizing the components in a optimized way and integrating docker-compose tool. Made efforts in solving issues interrupting the project flow. Performed load testing on API server using locust framework and eventually optimized the server by integrating a WSGI which can take traffic about 4 times better than before. Came up with a kubernetes architecture and further written configurations for Bassa API server, Aria2c and Web aligning to the design. Worked on updating the documentation and building a static site for showcasing Bassa.



### What Covered
1. Scripted a single dependency installation shell script across various operating systems. [`PR`](https://github.com/scorelab/Bassa/pull/715)
2. Optimized Travis CI builds. [`PR`](https://github.com/scorelab/Bassa/pull/754)
3. Hunted down various bugs interrupting the project flow. [`PR 1`](https://github.com/scorelab/Bassa/pull/744)  [`PR 2`](https://github.com/scorelab/Bassa/pull/742) [`PR 3`](https://github.com/scorelab/Bassa/pull/792) 
3. Containerized Bassa's Web, API, Database and Aria2c servers using Docker. [`PR 1`](https://github.com/scorelab/Bassa/pull/797) [`PR 2`](https://github.com/scorelab/Bassa/pull/793) [`PR 3`](https://github.com/scorelab/Bassa/pull/789) [`PR 4`](https://github.com/scorelab/Bassa/pull/782) [`PR 5`](https://github.com/scorelab/Bassa/pull/776) 
4. Integrated docker-compose tool for production and development. [`PR`](https://github.com/scorelab/Bassa/pull/793) 
5. Performed load testing on API server using locust framework. [`LINK`](https://bit.ly/2ElDJYr) 
6. Scaled Bassa API server to work with heavy traffic by integrating WSGI, Supervisord and Nginx. [`PR`](https://github.com/scorelab/Bassa/pull/813) 
7. Written configurations for deploying Bassa API server, Aria2c and Web containers over a Kubernetes cluster.[`LINK`](https://gist.github.com/kmehant/e8286ceca2aa66174e6e59bca6c19449)
8. Updated Bassa documentation [`PR`](https://github.com/scorelab/Bassa/pull/821) 
9. Designed a static documentation site for Bassa using Hugo framework.
[`PR`](https://github.com/scorelab/Bassa/pull/813) 

### What left
I would like to test the kubernetes cluster and further optimize it's configurations.
I would like to deploy Kubernetes cluster using AWS EKS service, Kops and Terraform.


### After the GSoC
Would like to take care of Bassa repository and would continue to commit.

### Reference
#### [GSoC Log Book](https://docs.google.com/document/d/1LrXeS_2KQtGNFjZpw3-Mj6wWubP5TMvm_7lc8k8obag/edit?usp=sharing)
