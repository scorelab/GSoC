# Soundcom

## Student Info
* Name : Piyush Singhal
* Email : singhalpiyush12@gmail.com
* Contact No. : (+91)8126141161
* University : Indian Institute of Technology Roorkee
* Github : https://github.com/singhalpiyush12


### Project Abstract
Soundcom is an open source android based app focussing on near field communication through soundwaves. At the moment it can be used to chat within a range of few meters where user can receive and broadcast messages. Low frequency waves have high attenuation in air but they also have long wavelengths which can be used be used by navies to communicate with submarines. This project helps you understand general wireless communication procedure and modify it according to use.


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4619289777143808)

### [GSoC Project Proposal](https://docs.google.com/document/d/1qIofVVXrrT2igRucCMwTHAL9sJZPFY692SvkAqaPlaY/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/soundcom)

### [GitHub Personal Repo](http://github.com/singhalpiyush12/soundcom)

### [Commits during GSoC 2018](https://github.com/singhalpiyush12/soundcom/commits/master)

### [Project Demo Video](https://drive.google.com/file/d/1QSEJx1tP35t-_ZtvqYZ-KsA3ZNMTRbLB/view?usp=sharing)

### [Project Wiki](http://github.com/scorelab/soundcom/wiki)

### [GSoC Blog](https://medium.com/@piyushsinghal/gsoc18-with-sustainable-computing-research-score-lab-6ebe42635a05)

### Work Summary
In the beginning of the project it was decided to make a react-native app. I started looking for libraries of sound analysis in react but couldn't find one. I then tried to create one using basic js libraries but failed. I found the library in android suitable for my use so I moved to android app. I had options to choose software for app development, Android Studio was the best with proper documentation of every feature. I made some tweaks in the library like increasing amount of data exchange and reducing time for the exchange. Then compiled the library and included it in my project. Next I created the complete UI of the app excluding chat feature. I was asked by my mentor to create a chat feature for the app. For chat we needed unique identity so I extracted user info from google accounts. I thought of creating a firebase database for chat storage and started working on it. Later I realised that this app is an offline app using internet will finish the meaning of the app. I made models for my message type and methods to display it. Initially messages were stored in message_list which was created at runtime. So chat would only store the messages which were exchanged at runtime. Once the app was closed all data was wiped. Then I thought of creating an offline database in internal storage, JSON was the simplest of all I can think of. I made a class to convert my message data to JSON format. First I have to check if the json file exists, if not then create one, if yes then read and write the file. Last task was creating testing of the app and adding readme to the project. Testing was a tough task I was able to write only few cases. Tests include message data check, Transmitted text length check, Button functioning test, message to JSON class test. Next I was working on internal file test but was not possible because test creates file in different folder and app checks for it in other one. Finally, I created Readme, wiki and added comments to the modules.

### What Covered
* Android Library for basic text exchange between two devices using sound waves.
* UI of the app.
* Chat storage in local json file.
* Extraction of user info from google accounts.

### What left
It is almost finished. More research can be done on increasing efficiency by changing method of modulation, restricting the data type to alphanumeric may increase accuracy of signal reception.   

### Reference
* Android Developer Documentaion has covered most of the part - https://developer.android.com/docs/
* For Chat implementation I looked at some blogs.
* So much work has been done on android and for your every need there is a blog available.

