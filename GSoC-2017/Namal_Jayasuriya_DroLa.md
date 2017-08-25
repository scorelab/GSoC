# DroLa

## Namal Jayasuriya
e.n.jayasuriya@gmail.com

### Project Abstract
A secure drone monitering system for a central authority Using LORA. Each drone has a externaly mounted unit on it. It transmit it's location and time ina secure way when flying. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5995323712339968)

### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/5863729068507136_1491227001_DroLaproposal_.pdf?Expires=1503747614&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=I6S94JK%2F46hxAXRjdLnrRMGkxngUikM2hBL61Dt6P9nZNQztrw6ZNVdrQdhaZf7staD2uzC8ymc21V0eVW4ih76YWeKjNioLsQ7TkDM3PUDg9KpOp557MqGm5CRV4A3VSbecFgpoBqj%2FsFmLgA8lqGiQB%2F2ZzMFY1ZFWbhQAT2FZ76Rlhzqb2lGBnpP52HMrcka7kd6oG0pClUCsKrhya3LQIg9VK2qbwpbqM5EEwuJV%2B8MrzE%2BGeLsH1P4wfnRVyDkYwCDf%2BXYq00c%2BKALBfCsWI7q7sF%2BD04KfJcfF7F4ZAbVEGaxZL61Ha6sQVCx2EmTCpnEyri9ztYj4zU2zkw%3D%3D)

### [GitHub Organization Repo](https://github.com/scorelab/drola)

### [GitHub Personal Repo](https://github.com/NamalJayasuriya/drola)

### [Commits during GSoC 2017](https://github.com/NamalJayasuriya/drola/commits/master)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](http://github.com)

### [GSoC Blog](http://GSoCBlog)

### Work Summary

Built a secure drone monitering system. Central authority can monitor the locations of each registered drone in a secured way.(At the proposal I proposed RSA security but with the limitations of microcontroller hardware I implemented AES security algorithm for this project. According to the requirement AES is secure enough.) 

I built a server system and browser application to the Central authority.

Designed a hardware unit and built thr firmware for the end node.

Design a effient message protocol for the system.


### What Covered

Web server and web Apllication Client to monitor drones.

Api to get drone locations from serial port and send them to browser applications.

End node Hardware module.

End node Firmware.

Base node Hardware module.

An effient message protocol.


### What left

Trusted Key Zone implementation for End Node.

Browser Application improvements.

Key Generation and Key transformation(to end node trusted zones) tool for base Node.

### Reference
