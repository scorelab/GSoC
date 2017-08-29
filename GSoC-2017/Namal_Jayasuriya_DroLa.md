# DroLa

## Namal Jayasuriya
e.n.jayasuriya@gmail.com

### Project Abstract
A secure drone monitering system for a central authority Using LORA. Each drone has a externaly mounted unit on it. It transmit it's location and time in a secure way when it is flying. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5995323712339968)

### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/5863729068507136_1491227001_DroLaproposal_.pdf?Expires=1504085190&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=E2A9q3TUup7dMoldvkhk7F97bHU71I03harb6KsCAziv%2Fe1IgZWG3t5rTlUPZcX7Ww4wTSoyPhWPmaO5P95LUg6H6CE%2FtkD2RG7LOwB7EeeJVME3CXX30HiOihkTHAZ39kITmOL1QF2%2FPVVeryaPBPsTsH9ENkzue3%2BQuYB8qAUMs02zKhZ4uONFjfcNeh1pYH0L5hOsSM9%2B21CD2smlw4CEB96eiGZum00ABXkQ%2BdrFDVlI1N3tF6jOhC2xxk6VfVELvpXzxM6ofcQeDwrYdKz1lvhcNYK3F2aluFng20u1kE%2BVuyaYQOhEL6KeFvs4ZA1olt%2FxHUCOVCFqdbvQgw%3D%3D)

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
