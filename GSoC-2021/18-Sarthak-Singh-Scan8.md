# Scan8

## Student Info

* Name - Sarthak Singh
* Email - sarthaksingh0900@gmail.com
* Github Profile - <https://github.com/sarthaksingh18>
* Medium - <https://medium.com/@sarthaksingh0900>
* Linkedin - <https://linkedin.com/in/sarthaksingh18>

## Project Abstract

Scan8 is a Kubernetes based rapid URL/file scan system that allows users to submit a list of files and take out the scan results.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4781449967828992)

## [GSoC Project Proposal](https://drive.google.com/file/d/1jmdfi5HNK263QtBoNnKRQPQ1tppVDGG_/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/Scan8)

## [GitHub Personal Repo](https://github.com/SarthakSingh18/Scan8)

## [Commits during GSoC 2021](https://github.com/scorelab/Scan8/commits?author=SarthakSingh18)

## [Project Demo Video](https://drive.google.com/file/d/1JFwxHgJTyqBNyQS9f-8gbW9ltup5Nzhh/view?usp=sharing)

## [Project Wiki](https://maanas-talwar.github.io/Scan8/)

## [GSoC Blog](https://medium.com/@sarthaksingh0900)

* Community Bonding
  * [Journey to GSoC'21](<https://medium.com/scorelab/journey-to-gsoc-2021-e6686618fd64>)
  * [Community Bonding Second Week](<https://medium.com/scorelab/gsoc21-second-week-5d0b030422a6>)
  * [Community Bonding Third Week](<https://medium.com/scorelab/gsoc-21-community-bonding-third-week-d39bfa958b70>)
* Coding Phase
  * [First Week](https://medium.com/scorelab/gsoc21-coding-phase-first-week-cc998b402311)
  * [Second Week](https://medium.com/scorelab/gsoc21-coding-phase-second-week-eb206554b8cf)
  * [Third Week](https://medium.com/scorelab/gsoc21-coding-phase-third-week-2766ce419021)
  * [Fourth Week](https://medium.com/@sarthaksingh0900/gsoc21-coding-phase-fourth-week-ba0a1028b97e)
  * [Fifth Week](https://medium.com/scorelab/gsoc21-coding-phase-fifth-week-397a449851)
  * [Sixth Week](https://medium.com/scorelab/gsoc21-coding-phase-sixth-week-ce51d4ce9e5b)
  * [Seventh Week](https://medium.com/scorelab/gsoc21-coding-phase-seventh-week-121fea4f3a87)
  * [Eighth Week](https://medium.com/scorelab/google-summer-of-code-eighth-week-827ab23b9a37)
  * [Ninth and Tenth Week](https://medium.com/scorelab/google-summer-of-code-ninth-and-tenth-week-58db29235278)
  
## Work Summary
 
During GSoC’21 I have worked upon the deployment part of the Scan8 project. In the first half of my GSoC journey, I have worked on collecting the required materials and published blogs for the topics that are required to deploy the Scan8 application.

 1. Comparison between Self Hosted database and Cloud provider database.

 2. Comparison between different CI/CD tools and discussed with the mentors and chosen the appropriate one which suits our use case.

 3. Secrets, ConfigMaps and environment variables and their use in the scan8.

 4. For hosting the database in k8s and the use of stateful sets in it.

 I have also created 3 different docker images of ClamAV with Debian, ubuntu and alpine and tested these images on different parameters such as CPU utilization, memory consumption and network IO by downloading 100 viruses from malware bazaar and running clamdscan on the files and for this, I have written 3 different shell scripts. All the images which are created have scored a 99% efficiency score with the dive tool.

In the second half of the GSoC’21, I have the first dummy up the architecture with help of different images such as Nginx, busy box etc after approval I have taken the application and created the deployment by writing the required deployment files and their services. Later I have integrated helm charts and used an umbrella chart to package the application.
Apart from this, I have tested docker images by creating containers and running them on the same network with mounted volumes.

![Deployment image](https://user-images.githubusercontent.com/46760104/127546528-fd0350ca-f308-4cf9-93a7-9995d5c6a330.png)

## What Covered

* Three different Docker files of ClamAV on Debian, Ubuntu and Alpine.
  * [#41](https://github.com/scorelab/Scan8/pull/41)

* Testing of images using shell scripts by downloading 100 viruses from malware bazzar and running clamdscan on it.
  * [#47](https://github.com/scorelab/Scan8/pull/47)

* Dummy Deployment by using Nginx image and alpine.
  * [#51](https://github.com/scorelab/Scan8/pull/51)
![Dummy deployment](https://user-images.githubusercontent.com/46760104/125098149-6b31cd00-e0f4-11eb-9a79-43b08bd06e0a.png)
* Deployment of Scan8 on local kubernetes enviornement.
  * [#59](https://github.com/scorelab/Scan8/pull/59)

* HPA for worker node.
  * [#62](https://github.com/scorelab/Scan8/pull/62)

* Helm charts umbrella deployment. 
  * [#70](https://github.com/scorelab/Scan8/pull/70)

* Readme files and structure representation of deployment.
  * [#71](https://github.com/scorelab/Scan8/pull/71)

* Blogs and notes on required topics.
  * [Comparison between Self Hosted Database and Cloud Provider Database Service.](https://medium.com/scorelab/comparison-between-self-hosted-database-and-cloud-provider-database-service-672626341448)
  * [CI/CD Tools](https://medium.com/scorelab/ci-cd-tools-c2d3242b7815)
  * [Secrets, ConfigMaps and Environment variables](https://medium.com/scorelab/secrets-configmaps-and-environment-variable-73cfe2c82d0c)
  * [StatefulSet in K8s](https://medium.com/scorelab/statefulset-in-k8s-24a0b3a30ec9)

## What left

Although I have completed almost all of the pre-decided milestones few topics are postponed to after GSoC.

* Integration of CI/CD in the project.
* Deployment of scan8 in GKE.

## Future Goals

* Proposing an Idea of creating public API endpoints by which anyone with the API key can scan the file passed in the body.
* Publishing helm package of the application which can be easily integrated with the applications and run as a service.
* Completing goals that are left.
* Reducing image size by removing virus definitions database from the image to the PV which can be shared by the multiple running worker pods and leads to reduced image size.
