# Bassa : Making installation of Bassa and containerize in a better way with efficient file storage server

## Student Info
- Name : Pawan Bhadu
- Email : bhadup21@gmail.com
- University : Indian Institute of Technology, Roorkee
- GitHub handle : https://github.com/demon-36
- LinkedIn profile : https://www.linkedin.com/in/pbhadu21/

### Project Abstract
Bassa is an automated download queue web-app. Bassa has been integrated with an open source storage server(Minio) and its file management system is improved than before, further Minio can be deployed as cloud storage server for Bassa, containerization of Bassa is also done using Docker and Docker-compose and Bassa containers can be deployed over Kubernetes for enterprise uses.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4681470927437824)

### [GSoC Project Proposal](https://docs.google.com/document/d/1_GQbaL_MGeXCg68zDb2vCcv8vj3vowemhWKLhI68M2s/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/Bassa)

### [GitHub Personal Repo](https://github.com/demon-36/Bassa)

### [Commits during GSoC 2019](https://github.com/scorelab/Bassa/pulls?q=is%3Apr+author%3Ademon-36+label%3AGSoC-2019)

### [Project Demo Video](https://drive.google.com/file/d/12jMXkuwwNm22M4EdkRNmEChoyIiPRf_o/view?usp=sharing)

### [Project Wiki](https://github.com/scorelab/Bassa/wiki)

### [GSoC Blog](https://gist.github.com/demon-36/f9004033446730a08b683abaa98f370f)

### Work Summary
Integrated an open source storage server(Minio) with Bassa for efficient file management which will have many functionality like file uploading, downloading, sharing and it can process files having size upto 5Tb individually. Fixed some UI issues faced during project, updated installation scripts and documentation of Bassa and worked on containerization of Bassa and wrote configuration files of Minio for Kubernetes deployment.

### What Covered
1. Integrated file storage server with Bassa
2. Updated installation scripts of Bassa for installation on various OS flavors
3. Fixed UI issues of Bassa which were disturbing work flow
4. Tested and updated Dockerfiles for Bassa API and Minio
5. Tested and updated Docker-compose for Minio integration
6. Updated documentation of Bassa
7. Composed kubernetes configuration file for Minio 

### What left/ After GSoC
1. Testing and optimization of Kubernetes configurations
2. Testing deployment of bassa over kubernetes cluster.

### Reference
- [Minio storage server](https://github.com/minio/minio)
- [Kubernetes](https://kubernetes.io/docs/home/)
- [GSoC LogBook](https://docs.google.com/document/d/13U4HWiwgRoUPLc6zr5opkv1D6Hi1TDZWKct_GKlsv_0/edit?usp=sharing)
