# Project Name
SenZ Switch

## Student Info
* <b>Name</b> : Sumedhe Dissanayake
* <b>Email</b> : [sumedhedissanayake@gmail.com](mailto:sumedhedissanayake@gmail.com)
* <b>Github</b> : [https://github.com/sumedhe](https://github.com/sumedhe)
* <b>Linkedin</b> : [https://www.linkedin.com/in/sumedhe](https://www.linkedin.com/in/sumedhe)
* <b>Institute</b> : University of Colombo School of Computing, Sri Lanka.


### Project Abstract
SenZ Switch is a high-speed message passing system which can be used to do the communicating between IoT devices. After connecting the devices to the system, they can share data with the other connected devices. The system acts like a message broker and it does not keep or read any data passing through it. All the messages passing through the system are secured with an End-to-end Encryption method. So this system to can be used to connect private devices also without hesitating.


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6441506961883136)

### [GSoC Project Proposal](https://drive.google.com/open?id=1H_gOvQTQoHPOiBmdKv65zb3ADAw84eup)

### [GitHub Organization Repo](https://github.com/scorelab/senz)

### [GitHub Personal Repo](https://github.com/sumedhe/senz)

### [Commits during GSoC 2018](https://github.com/scorelab/senz/commits?author=sumedhe)

### [Project Demo Video](https://youtu.be/QXyGK5AwvFI)

### [Project Wiki](https://github.com/sumedhe/senz/wiki)

### Work Summary

For GSoC 2018, I have implemented the main functions of the SenZ switch using Scala. The SenZ switch works as a hub and it passes messages between devices. Akka actor models are used for connecting devices with the server and passing messages between devices. Sample client programmes are also implemented to transfer data between devices with end-to-end protection.

### What Covered
Things covered in GSoC coding period
- Senz message parser to parse message queries
- TCP Socket
- Akka models for device sessions and the socket
- RSA Key Generation module
- Session manager to handle connected devices
- Database module to use mongodb
- Message data encryption using AES Crypto
- Client programs to transfer images between two devices
- Unit tests for each module
- API Documentation


### What left
- Admin panel to manage devices
- Streaming functionalities

### Reference
1. [Akka official Documentation](https://akka.io/docs/)
2. [Scala Documentation](https://docs.scala-lang.org)
3. [Modern Functional Programming and Actors With Scala and Akka](https://pdfs.semanticscholar.org/1f1e/398b39a77681e0c83feb12e2bcdace133728.pdf)
4. [Azure IoTHubReact](https://azure.github.io/toketi-iothubreact)
5. [MySensors.info](http://mysensors.info/senz.html)
