# Project Name

Drola - Backend with Realtime Database

## Student Info

* Name		: Janagan Sivagnanasundaram
* LinkedIn	: https://www.linkedin.com/in/janagan-sivagnanasundaram-806a755a/
* Github  	 : https://github.com/janagan1993
* Email     	: janagangsoc@gmail.com

### Project Abstract

Redesign and Implement the DroLa system as a real time database based system instead of  WebSocket based system. Introduced bi-directional end-to-end secured communication between sensor nodes and Application Server. A new packet structure with the binary level message header, header parser and message parsers to make the system more general to use as a general tracking system.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4693073825628160)

### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/6649662954536960_1522148301_GSOC_2018-Proposal.pdf?Expires=1534334000&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=OKFD9hJ3%2FWlvqHkNsN2ELMEwfiQreJhMNwFqBeMQuD2%2B1sBrVuBndXQW1xhgwD0EFbInhjjbPbMNfmb%2BOlLMAiGLGhOWnv6t0dmGuIWnSLiJl4hiy33px6Zq1XPMmrq6Pz5GRc8dS%2F3l181tFY0IPzWzjU4LSxBHjmgDsOCrOqVZvszAWGucvjis8InPAnBA%2FiMNmWeSuY7PRMInuC3WHLhzgr5mZrYWHjdMpntee2SaxNaGafDKtyylh2X2wovDAe2%2B3Emne0cP2yaxU336TPIFeMrJoqnTBzOJh5VUPG5q4SI0AcqtOn9eN%2F0ruTLtJxovUPuE%2B5WV%2ByLO9KBs9g%3D%3D)

### [GitHub Organization Repo](https://github.com/scorelab/drola/tree/general-develop)

### [GitHub Personal Repo](https://github.com/janagan1993/drola/tree/drola_generalized)

### [Commits during GSoC 2018](https://github.com/scorelab/drola/commits/general-develop)

<!--### [Project Demo Video](http://LinkToDemoVideo)-->

<!--### [Project Wiki](http://github.com)-->

### [GSoC Blog](https://letstartjana.blogspot.com/)

### Work Summary

* Integrated Mongo change stream replica database to notify Sensor node changes realtime.
* Bi-Directional communication using a new encription library(AES-256CBC) for Application server, LoRa Gateway and Sensor Node.
* Design and Implement a message protocol using byte level data encoding which suitable for LoRa packet limitation and Implement for Sensor Nodes, Lora Gateway and Application Server.
* Message Parser to give a general Application API.

### What Covered

* Real Time Database Integration .
* Bi-Direction secured End to End communication from Sensor Node to Application Server.
* Design and Implemented message Protocol.
* Partially implemented Message Message Parser.

### What left

* Complete Message parser.

### Reference

- [MongoDB 3.6 change streams example with Node.js](https://medium.com/@thakkaryash94/mongodb-3-6-change-streams-example-with-node-js-2b9a85652c50)
- [An Introduction to Change Streams](https://www.mongodb.com/blog/post/an-introduction-to-change-streams)

- [DroLa : Master branch(Previous Project) ](https://github.com/scorelab/drola)

- [AES for microcontrollers](https://github.com/spaniakos/AES)

- [Node js Guides](https://nodejs.org/en/docs/guides/)

- [LoRa WAN : MOst widely Spreaded LPWAN ](https://lora-alliance.org/about-lorawan)

- [LoRa Device : E45-TTL-100 ](https://quadmeup.com/wp-content/uploads/2017/09/E45-TTL-100_Datasheet_EN_v1.2.pdf)







