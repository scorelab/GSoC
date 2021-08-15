# Scan8

## Student Info
* Name: Maanas Talwar
* Email: maanastalwar1@gmail.com
* GitHub: [maanas-talwar](https://github.com/maanas-talwar)
* Linkedin: [Maanas Talwar](https://www.linkedin.com/in/maanas-talwar/)
* Medium: [@maanas-talwar](https://medium.com/@maanas-talwar)

## Project Abstract
Scan8 is a distributed scanning system for detecting trojans, viruses, malware, and other malicious threats embedded in files. The system allows one to submit a list of files and get the scan results in return.  

The project is divided into various modules namely ```Dashboard```, ```Coordinator Node```, ```Worker Node```, and ```Testing```.  
The ```Dashboard``` provides a responsive web interface for uploading files for new scans and tracking the status of all the submitted scans.  
The ```Coordinator Node``` listens to updates for new scans, subsequently creating and adding scan jobs to the Redis Queue.  
The ```Worker Node``` listens to updates for new jobs in Redis Queue and executes them.  
The ```Testing``` module helps in maintaining the application and facilitating the CI/CD process for the same.


## GSoC Project Page
* [GSoC 2021 with SCoRe Lab](https://summerofcode.withgoogle.com/projects/#6676343485366272)

## GSoC Project Proposal
* [Scan8 project proposal](https://drive.google.com/file/d/1KC0fnGLpaqUaH5kz2LviQ5jYkHOkmMIq/view?usp=sharing)

## GitHub Organization Repo
* [scorelab/Scan8](https://github.com/scorelab/Scan8)

## GitHub Personal Repo
* [maanas-talwar/Scan8](https://github.com/maanas-talwar/Scan8)

## Commits during GSoC 2021
* [maanas-talwar/Scan8/commits](https://github.com/maanas-talwar/Scan8/commits/main?author=maanas-talwar)

## Project Demo Video
* [Introduction](https://drive.google.com/file/d/16oXRxPhDIK1QnPnjoJig_SXpZj8Lj-mq/view?usp=sharing)
* [Application Demo](https://drive.google.com/file/d/1TblQdpIAS4VybZzgb2ORfmJiXs_McVrO/view?usp=sharing)
* [Testing Demo](https://drive.google.com/file/d/1CTvLrD_fSdq6xxXabgkLGOPs3jDLwPrT/view?usp=sharing)

## Project Wiki
* [Scan8](https://maanas-talwar.github.io/Scan8/)

## GSoC Blog(s)
* [GSoC’21: The onboarding phase](https://medium.com/scorelab/gsoc21-the-onboarding-phase-71d5e82892d6)
* [GSoC’21: Scan8 building blocks](https://medium.com/scorelab/gsoc21-scan8-building-blocks-d26c1b2c2c9b)
* [GSoC’21: Scan8 Application Architecture](https://medium.com/scorelab/gsoc21-scan8-application-architecture-bfbf53714645)
* [GSoC’21: Scan8 user interface](https://medium.com/scorelab/gsoc21-scan8-user-interface-2331eeea4272)
* [GSoC’21: Scan8 server-side operations](https://medium.com/scorelab/gsoc21-scan8-server-side-operations-baf9c5d57ed0)
* [GSoC’21: Scan8 server-side operations cont.](https://medium.com/scorelab/gsoc21-scan8-server-side-operations-cont-22cf42290212)
* [GSoC’21: Scan8 coordinator node](https://medium.com/scorelab/gsoc21-scan8-coordinator-node-70143adadafc)
* [GSoC’21: Scan8 worker node](https://medium.com/scorelab/gsoc21-scan8-worker-node-e53c45137648)
* [GSoC’21: First evaluation](https://medium.com/scorelab/gsoc21-first-evaluation-5ad6b2248234)
* [GSoC’21: Application testing aspects](https://medium.com/scorelab/gsoc21-application-testing-aspects-e12aa11019a)
* [GSoC’21: Refactoring code and formalizing unit tests](https://medium.com/scorelab/gsoc21-refactoring-code-and-formalizing-unit-tests-dd337f9352e1)
* [GSoC’21: Developing the test suite](https://medium.com/scorelab/gsoc21-developing-the-test-suite-56c1f69bedb3)
* [GSoC’21: Scan8 test suite and documentation](https://medium.com/scorelab/gsoc21-scan8-test-suite-and-documentation-a999d9fbc26e)

## Work Summary
Scan8 is a distributed scanning system for detecting trojans, viruses, malware, and other malicious threats embedded in files. The system allows one to submit a list of files and get the scan results in return. Being a new project, the main objectives were to come up with an efficient system architecture/design and then implement the same.  
The project was divided into 2 phases: 
1. Application designing and implementation
2. Building a test suite to fascilitate the CI/CD pipline

During the GSoC period, I designed the application architecture from ground up, put the design into practice via quality code, developed the test suite for the same, and worked on the documentation in the form of a README and a [github page](https://maanas-talwar.github.io/Scan8/).  

**Application architecture**:
![Scan8 application architecture](https://user-images.githubusercontent.com/54113320/129450716-b98cd6ae-f2b9-4e5f-9fb6-fc8c96b0ee47.png)

## What Covered
Please find below the summary of my contributions to the Scan8 project during GSoC 2021.
* Developed a responsive web interface for the application dashboard in sync with the database using HTML, Bootstrap and Javascript. [[PR-1]](https://github.com/scorelab/Scan8/pull/34) | [[PR-2]](https://github.com/scorelab/Scan8/pull/35) | [[PR-8](https://github.com/scorelab/Scan8/pull/61)]
* Developed the back-end infrastructure using MongoDB with Flask for implementing various routes(including storing files to the server) and extracting meta-data, while connecting it to the user interface. [[PR-3]](https://github.com/scorelab/Scan8/pull/37) | [[PR-4]](https://github.com/scorelab/Scan8/pull/44)
* Developed the Coordinator node scripts to create and add ClamAV scan jobs to the Redis Queue. [[PR-5]](https://github.com/scorelab/Scan8/pull/48)
* Developed the Worker node scripts to run the Redis worker and execute the jobs enqueued by the Coordinator node with a provision for resubmission of failed scans and a timeout. [[PR-6](https://github.com/scorelab/Scan8/pull/53)]
* Created a local setup and usage guide. [[PR-6](https://github.com/scorelab/Scan8/pull/53)]
* Developed a module to convert and store scan results to a JSON. [[PR-6](https://github.com/scorelab/Scan8/pull/53)]
* Refactored the code for better maintainability and to ease the process of creating Docker images. [[PR-7](https://github.com/scorelab/Scan8/pull/56)]
* Developed the test suite for the application. [[PR-9](https://github.com/scorelab/Scan8/pull/65)] | [[PR-10](https://github.com/scorelab/Scan8/pull/69)]

## What left
Following tasks were not strictly a part of my proposal, if added will enhance the overall project quality.
* Setting up a cluster health monitoring dashboard using Prometheus (*Stretch Goal*).
* Adding more test cases to the test suite will help in identifying potential errors (if any) before deploying to production.
