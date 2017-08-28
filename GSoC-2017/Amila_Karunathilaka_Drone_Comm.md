# Drone Comm

## Student Info
* Name - K. A. De Zoysa Karunathilaka
* Country - Sri Lanka
* University - University of Moratuwa
* Field of study - Computer Science & Engineering
* GitHub - https://github.com/Amila1991
* Email - amilakarunathilaka.12@cse.mrt.ac.lk
* Contact No. - +94779386412

### Project Abstract
Drone Comm is community platform which is help to meet drone owners and drone required people. using this platform drone required people can request drone from the community. And drone pilot who has drone can be hire their drones and can get income. In this case drone requester publish he/she task(purpose) description and request drone through this community platform. These open task request forward to drone pilot and drone pilot bid for these task.

### [GSoC Project Proposal](https://docs.google.com/a/cse.mrt.ac.lk/document/d/1Pj5INineHwD-yIHs4ibBRlRCJnYPRDlgZC8zREV_nr8/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/Drone-Comm)

### [GitHub Personal Repo](https://github.com/Amila1991/Drone-Comm)

### [Commits during GSoC 2017](https://github.com/scorelab/Drone-Comm/commits/master)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/Amila1991/Drone-Comm/wiki)

### [GSoC Blog](https://medium.com/@amilakarunathilaka.12/gsoc-experience-e823aa4e0165)

### [API Documentation](https://drive.google.com/open?id=1hbae5COEZc82dPIb3Jp3H5eDjJp8n1SFj0j6_l1avbU)

### Work Summary
Developed Drone Comm as project of Google Summer of Code 2017.

This is new concept given by. SCoRe lab organization. First I started to designed project architecture. In this case I have decided to implement seperate backend and frontend. In implementation phase first I have developed backend. Drone Comm backend has RESTful API. This API exposes Drone Comm services. Frontend web application consume these backend REST API. 

Nodejs used to developed backend implementation and backend REST API structure built using Express Framework. I used MongoDb to persist Drone Comm data like user detail, drone detail & drone task detail. This is Drone Comm backend setup.

Angular 4 used to develop frontend web application. This frontend web app has Drone Comm user interfaces. These interfaces communicate with Drone Comm Backend.

In this GSoC period I have done above mention things.

### What Covered
* Designed system archiitecture
* Implemented backend services
* Backend services used MongoDB get and persist to the system data. In this case used Mongoose ORM to communicate between MongoDB database and backend REST API services.
* JSON Web Token(JWT) used to managed Drone Comm System authentication and authorization.
* Implemented queue based message passing pattern to notify newly added drone tasks to drone pilots. 
* Frontend include log in, registration, drone create, create drone task ...etc. These UI component implemented in frontend web application.

### What left
* Bid or response for drone tasks.
* Private chat between users.(most of time private chat between drone client and crone pilots).
* Do Payment through Drone Comm.

### Reference
* [Nodejs Express Framework](https://expressjs.com)
* [Angular 4 Framework](https://angular.io)
* [Mongoose ORM](http://mongoosejs.com)
