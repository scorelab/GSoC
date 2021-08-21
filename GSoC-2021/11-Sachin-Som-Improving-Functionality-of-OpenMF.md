# Improving Functionality of OpenMF

# Student Info

- Name : Sachin Som
- Email : sachinsom507@gmail.com
- Github : [sachinsom93](https://github.com/sachinsom93)
- Medium : [sachinsom507](https://medium.com/@sachinsom507)
- LinkedIn : [sachinsom507](https://www.linkedin.com/in/sachinsom507)

# Project Abstract

![OpenMF Logo](https://github.com/scorelab/OpenMF/raw/master/Logo.png)

OpenMF is an open source forensic tool for Android smartphones that helps digital forensic investigators throughout the life cycle of digital forensic investigation.

For e.g. let us say we have a crime scene in which we have captured some suspects and we have their mobile phones. If we want to extract all the data from their phones and see which of them are actually involved in the crime scene then we require a software to perform this task and produce Meaningful evidence and Analysis report for every phone (Digital forensic case). The OpenMF project is a dedicated software to:
- Extract the relevant data
- Manage all the cases separately
- Produce Analysis report

This open source project is an important tool for Digital forensic organization. At present OpenMF is only a commmand line tool but we are planing to make a complete web client with additional features like Admin, Management and Extractor. These roles will have different privileges to the tool and as a whole it will become a complete open source forensic tool for Android smartphones which then can be used by any Digital forensic investigation organization.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4970501744623616)

## [GSoC Project Proposal](https://docs.google.com/document/d/1evOmzZdmDTkwfGoygm_C35S1h7_ekLFYf1CTwi5i8rw/edit?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/OpenMF)

## [GitHub Personal Repo](https://github.com/sachinsom93/OpenMF)

## [Commits during GSoC 2021](https://github.com/scorelab/OpenMF/commits?author=sachinsom93)

## [Project Demo Video](https://drive.google.com/drive/folders/1VIV19zDzC-MK1R3qS2C7rQZljp0fFOCO?usp=sharing)

## [Project Wiki](https://github.com/scorelab/OpenMF/wiki)

## [GSoC Blog](https://medium.com/@sachinsom507/list/my-journey-of-gsoc-2021-df779092e930)

# Work Summary

* Design and modify existing database architecture.
* Refactore flask backend design and structure.
* Create REST APIs for User Authentication.
* Implement User authentication in Frontend.
* Create `Admin` specific REST APIs.
* Develop Frontend section for `Admin` User.
* Design and Implement feacture for storing and displaying all the cases's directories in hieararchical manner inside `Management` Section.
* Create `Management` Specific REST APIs and Develop Frontend Section for `Management` User.
* Implement `Data Extraction` feacture in Frontend along with `Extractor` Frontend section.
* Data Visualization on extracted data of rooted Android Device.
* Implement addional Feature like forgot password, verify password etc.
* Work on some existing bugs.
* Update Readme according to updated project structure.
* Write Weekly Blogs.


# What Covered
**Week 1**
  * Designed and Implemented database architecture having   seperate modal classes for each entitiy i.e. `Admin`, `Extractor`, `Management`, `Cases` and `Tasks`.
  * Refactored flask backend structure of OpenMF.
  * Refactored existing APIs incorporating newly designed database architecture and flask structure.
  * **Related PR**
    * [Refactor flask-backend structure #171](https://github.com/scorelab/OpenMF/issues/171)
    * [Revamp Database Architecture #172](https://github.com/scorelab/OpenMF/issues/172)

**Week 2**
  * Implemented Authentication routes using `JSON WEB TOKEN`.
  * Developed authentication login and signup process in frontend using authentication routes.
  * **Related PR**
    * [[Backend] Implementing JWT and creating decorators for each role #179](https://github.com/scorelab/OpenMF/issues/179)
    * [[Frontend] Integrating Auth process with Frontend #183](https://github.com/scorelab/OpenMF/issues/183)

**Week 3**
  * Created `Admin` Specific REST APIs, as following
    * User management APIs
        - API for fetching profile details of admin
        - APIs for creating new members(extractor and management), listing all members, updating the role of a member and deleting a member account.
    * Task management APIs
        - APIs for creating and assigning a new task,   deleting a task, re-assigning a task and fetching all the completed and uncompleted tasks.
    * Data management APIs
        - API for fetching all the extracted case list and listing all the connected active devices.
   * **Related PRs**
     * [[Backend] Creating Admin Specific REST APIs #188](https://github.com/scorelab/OpenMF/issues/188)

**Week 4**
  * Developed Entire Frontend Section for `Admin`
    * Components for listing, editing and deleting both kinds of members i.e extractor and management.
    * Implemented create and add new member components.
    * Developed frontend pages to see active cases and tasks assigned to members(completed and uncompleted tasks).
  * **Related PRs**
    * [[Frontend]: Create Frontend Section for Admin #191](https://github.com/scorelab/OpenMF/issues/191)

**Week 5**
  * Created Frontend Section for `Management` member
    * Implemented some APIs related to `Management` member.
    * Developed Components for listing all extracted cases, rendering contents of a case directory in hierarchical manner etc.
  * **Related PRs**
    * [[Frontend]: Developing Frontend for Management Section #197](https://github.com/scorelab/OpenMF/issues/197)

**Week 6**
  * Extending frontend section for `Management` member created in week 5.
  * Implemented routes for showing all the files of each case directories.
  * Developed frontend for the same integrating above created APIs.
  * **Related PRs**
    * [Extending Management Frontend #203](https://github.com/scorelab/OpenMF/issues/203)

**Week 7**
  * Created Frontend Section for `Extractor` member.
  * Implemented Data Extraction part in Frontend by integrating data extraction API routes.
  * **Related PRs**
    * [[Code Quality]: Add Comments to functions, components and modules of Flask backend and React Frontend #204](https://github.com/scorelab/OpenMF/issues/204)
    * [[Frontend]: Develop Frontend Section for Extractor User #215](https://github.com/scorelab/OpenMF/issues/215)

**Week 8**
  * Performed Data Visualization for extracted data.
  * Created Bar, line, Polar etc charts for analysing browser history data.
  * **Related PRs**
    * [Data visualization #217](https://github.com/scorelab/OpenMF/issues/217)

**Week 9**
  * Created REST APIs for verify email address and forgot password.
  * Developed Frontend and integrated this with APIs for verify address and forgot password.
  * Worked on some bugs related to `Admin` Section.
  * **Related PRs**
    * [[Bug]: Modify Data Extraction For Tag Association #220](https://github.com/scorelab/OpenMF/issues/220)
    * [Email Verification and Forgot Password Implementaion #225](https://github.com/scorelab/OpenMF/issues/225)
    * [[Bug]: Need to replace data-grid with table pagination #227](https://github.com/scorelab/OpenMF/issues/227)

**Week 10**
  * Updated Readme for Frontend and backend section of OpenMF.
  * Created Videos regarding installation-setup and demos of frontend and backend sections.
  * Worked on some left over bugs.
  * **Related PRs**
    * [[Documentation]: Write Updated Readme For Flask Backend #232](https://github.com/scorelab/OpenMF/issues/232)
    * [Extract all data from rooted Android device not working #170](https://github.com/scorelab/OpenMF/issues/170)


# What left

I have successfully completed all the milestones decided for GSoC 2021. Altough following things could be added to enhance the scope of the project.

* Writting Unit Tests for React Frontend and Flask backend for identifying potential errors.
* Adding some more data visualisation charts for extracted data.