# Project Name

Bassa - Dockerize and modify features

## Student Info

- Name :Kaveesha Baddage
- Email :kbaddage98@gmail.com
- GitHub Profile :https://github.com/KaveeshBaddage

### Project Abstract

Bassa is an automated download queue which tries to minimize bandwidth wastage.Objectives of the project was dockerize Bassa project to simply run the project without complex configurations and fix bugs which caused to improper execution of the web application. I fixed several bugs and implemented several features in the project.

### [GSoC Project Page](https://summerofcode.withgoogle.com/dashboard/project/4885623415504896/overview/)

### [GSoC Project Proposal](https://docs.google.com/document/d/1qof_0eGaeYPTahNvu9YK_6TuFofjPqiaEbf7i4gOb_E/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/Bassa)

### [GitHub Personal Repo](https://github.com/KaveeshBaddage/Bassa)

### [Commits during GSoC 2017](http://github.com/commits)

- Resolving Issue #122 - Fix the bug which caused to admin panel cannot accessible after refresh the web page.
	- https://github.com/scorelab/Bassa/pull/134

- Implement new functionality to give system running configuration using single configuration file.
	- https://github.com/scorelab/Bassa/pull/133

- Implement Message handler function to avoid server crash when it handles multiple download requests.
	- https://github.com/scorelab/Bassa/pull/131

- Change data tranfering method for secure data trasfer in between frontend and backend.
	- https://github.com/scorelab/Bassa/pull/129

- Resolving Issue-#125 - Implement new feature to view current user's user name on logout menu.
	- https://github.com/scorelab/Bassa/pull/127

*Dockerizing the project - Implemented two Dockerfiles to run frontend services and backend services and run those files using docker-compose file. This function is partially completed.
	https://github.com/KaveeshBaddage/Bassa/tree/Dockerizing

### [Project Wiki](https://github.com/scorelab/Bassa/wiki)



### Work Summary

- Solved server crashing problem when it runs several download requests.
- Solved several bugs which caused to improper execution of the web application.
- Created new functionalities to enhance web application usability and performance.
- Partially done the dockerizing the project

### What Covered

- Resolved several bugs which caused to improper execution of the web application.
	- Fix authentication failure problem which caused to admin panel cannot accessible after refresh the web page.
	- Replace data tranfering variable types for secure data trasfer between backend and frontend
	
- Create new functionalities to enhance web application usability and performance.
	- Implement Message handler function which solves server crashing problem when it runs several download requests.
	- Create functionality to view current user on logout menu.
	- Create functionality to load system configuration using a single file.

### What left

Change the system routing which will support to run the system on docker containers
- Implemented two Dockerfiles to run frontend services and backend services inside two containers and implemented docker-compose file to connect those containers. Have to change system routing which will support to communicate between two containers and run the system inside those containers.


### Reference

- [Thread handling in python](https://docs.python.org/3/library/threading.html)
- [Access Java Web Token](https://jwt.io/)
- [Docker Documentation](https://docker-curriculum.com/#setup)

