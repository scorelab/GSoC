# Project Name
DroneSym - A realtime drone monitoring and controlling app
## Student Info
Name : Hasanga Somaratne
University : University of Colombo School of Computing
E-Mail : hasanga.charaka@gmail.com
### Project Abstract
DroneSym is a web app that allows simulating drone fleets and monitoring them in real time. Users are able to create new drone simulators, assign them a flightpath and issue commands.
### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4778065891688448)
### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/5790014544805888_1490973150_GSoCDroneSymproposal.pdf?Expires=1503543676&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=QvzhHhqVfYgwJnXfLosEuA9wlovFYfhbdEkmt%2BAMhKAPO%2FVwnA6QJdAlckrdn9cb2DvznB0pIBtxud9dtzYo2dM9nPpYLYjvKSNqI3Hpzesp8TPYvBBk36yACqSiYaJrWXtYv5U8WY1%2B%2FQVU52F5XZqTi%2BN2AJJFnPiaXI73CDoYp16dHGfWuQUVwoS2eUNqx9OG9b0I8wKm%2Bb6CEKMBZuQD8G8hFFgegJ6raSZaMf0MwrLMO9ywjNR66eAGgRmuF5mte0hlONPb78sIg1xU7A1baIauOWwxZl%2FbTgw5JQwrtr8ge8fUyyRB%2BfREMDCZA8MHIJhC6Dv420JljH76MQ%3D%3D)
### [GitHub Organization Repo](https://github.com/scorelab/DroneSym)
### [GitHub Personal Repo](https://github.com/hasa93/DroneSym)
### [Commits during GSoC 2017](https://github.com/scorelab/DroneSym/commits?author=hasa93)
### [Project Demo Video](https://drive.google.com/file/d/0B0xVuKx6qWJJQ0N1MTIyVXRValE/view?usp=sharing)

### [Project Wiki](https://github.com/hasa93/DroneSym/wiki)

### [GSoC Blog](http://GSoCBlog)

### Work Summary
DroneSym is a project started from scratch. As for now the drones controlled and monitored are simulations run through Dronekit-SITL module. The developing work on project required backend to handle user management, drone fleet management and real-time communication with simulated drone instances. On the frontend a dashboard and a map displaying drones is implemented. All communications with drones needs to be in real-time therefore websockets and real-time databases are needed to address the requirement.

### What Covered
- Create a Flask API providing an interface to Dronekit and Dronekit-SITL modules
- Implemented websocket channels for real-time communications through Socket.io and Firebase real-time database
- Implemented a REST API to interface between Flask API and Frontend
- Implemented JWT authentication and role based authorization
- Implemented the frontend user interface with Angular 2

### What left
- Add a user management module to create user groups and assigning them to drone groups
- Implement an abstract data-layer on top of Firebase and MongoDB
- Implement MAV commands routes to change airspeed and altitude

### Reference
[Dronekit Python API Reference](http://python.dronekit.io/automodule.html)