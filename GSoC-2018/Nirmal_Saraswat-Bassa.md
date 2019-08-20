# Bassa - Develop a mechanism to download file from server to local

## Student Info
  * Name - Nirmal Sarswat
  * Email - nirmalsarswat400@gmail.com 
  * University - Indian Institute of Technology, Roorkee
  * GitHub profile - https://github.com/vivonk
  * LinkedIn profile - https://www.linkedin.com/in/vivonk

### Project Abstract
Bassa is an automated download queue for enterprises use. If a software can download all your files in the background without keeping it open then it's all the best. Bassa can be used best if the Bassa will be a server where people can put the download in the queue and after some time your download is done. `Bassa still doesn't provide an option to download the file from the server. This project will lead to making files downloadable from the Bassa server in a single click`. After this target I made myself to do all the below tasks

   1. Changed the front end with download feature and implemented grid view of downloaded files
   2. Implemented file sending mechanism with concurrency handling
   3. Written compression module to send compressed file to user end when they hit for download
   4. Implemented file sharing system where user select some files and back end generates a link which contains all the files in a single compressed file
   5. Refactored back end API declarations, means separated endpoint declaration and implementation and refactored some files for ease of understanding

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5891538614222848)

### [GSoC Project Proposal](https://drive.google.com/open?id=1NjEIwYZ7idM4uETSQo5Jvzsv1lKWbg59jxBR8LtSNLU)

### [GitHub Organization Repo](https://github.com/scorelab)

### [GitHub Personal Repo](https://github.com/scorelab/bassa)

### [Commits during GSoC 2018](https://github.com/scorelab/Bassa/pulls?q=is%3Apr+author%3Avivonk+label%3AGSoC-2018+is%3Aopen)

### [Project Demo Video](https://drive.google.com/open?id=1xNJdTEzixJg1vUyRrkONfF0VbJliOzlQ)

### [Project Wiki](https://github.com/scorelab/Bassa/wiki)

### [GSoC Blog](https://groups.google.com/forum/#!forum/score-community)
I have updated my work details on common community group so that everyone be updated that what's going with the Bassa
Probably could be found on keyword search `Nirmal Bassa`

### Work Summary
Implementing Download feature was really exciting because it have many edge cases that you have to think for and have to make a solution for all the cases. So here are my things that I have implemented so far : 
* Download feature for single/multiple files where the files are compressed in a single file. [#464](https://github.com/scorelab/Bassa/pull/464), [#465](https://github.com/scorelab/Bassa/pull/465), [#472](https://github.com/scorelab/Bassa/pull/472)
* Files could be shared with a single link and link could be generated from front end it self. Whenever someone create a sharing link, it will compress those files in a single zip file and save it to tmp folder and when user hit that link, file will be sent. [#479](https://github.com/scorelab/Bassa/pull/479)
* Created a grid view of downloaded files on front end side for better look [#463](https://github.com/scorelab/Bassa/pull/463)
* Separated declaration of endpoints and it's logic, basically mappings are declared in a single module where logical parts are in different modules. [#475](https://github.com/scorelab/Bassa/pull/475)

After this work, Bassa is full with it's basic purpose which means now user can download the files which he/she put in queue to download. I have got many new skills like debugging, code styles, compression and much more.



### What Covered
1. Download feature
2. Sharing feature
3. Refactoring codebase
4. UI changes

### What left
* Update Bassa documentation
* Push develop branch commits to master

### After the GSoC
All the GSoC tasks are already done, just some extra tasks that I and my mentor agreed to do are in progress :)
* Replace gulp and bower by webpack - (Not GSoC task)
* Local file upload - (Not GSoC task)

### Reference
* ZLib - https://docs.python.org/3/library/zlib.html

* Flask - http://flask.pocoo.org

* AngularJs Documentation - https://docs.angularjs.org/guide

* AngularJs material library - https://material.angularjs.org/
