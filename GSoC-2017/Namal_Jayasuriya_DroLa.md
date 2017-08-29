# DroLa

## Namal Jayasuriya
e.n.jayasuriya@gmail.com

### Project Abstract
A secure drone monitering system for a central authority Using LORA. Each drone has a externaly mounted unit on it. It transmit it's location and time in a secure way when it is flying. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5995323712339968)

### [GSoC Project Proposal](https://docs.google.com/document/d/1-pXsKezPtq4lK4zOukn4ZdbWuOBoAXDFYSu32KRCHws/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/drola)

### [GitHub Personal Repo](https://github.com/NamalJayasuriya/drola)

### [Commits during GSoC 2017](https://github.com/NamalJayasuriya/drola/commits/master)

### [Project Demo Video](https://www.youtube.com/watch?v=1I--f2gv1WM&list=UUuT-aJUcxQLe6E5IRniEX6A&index=1)

### [Project Wiki](https://github.com/NamalJayasuriya/drola/wiki/Drola)

### Work Summary

Built a secure drone monitering system. Central authority can monitor the locations of each registered drone in a secured way.(At the proposal I proposed RSA security but with the limitations of microcontroller hardware I implemented AES security algorithm for this project. According to the requirement AES is secure enough.) 

I built a server system and browser application to the Central authority.

Designed a hardware unit and built the firmware for the end node.

Design a secure and effient message protocol for the system.


### What Covered

Web server and web client apllication to monitor drones.

Api to get drone locations from serial port, decrypt them and send them to browser applications.

End node Hardware module.

End node Firmware.

Base node Hardware module.

An effient and secure message protocol.


### What left

Trusted Key Zone implementation for End Node.

Browser Application improvements.

Key Generation and Key transformation(to end node trusted zones) tool for base Node.

### Reference
