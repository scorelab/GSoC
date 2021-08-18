# Improving Fuctionality of OpenMF

# Student Info

- Name : Sachin Som
- Email : sachinsom507@gmail.com
- Github : [sachinsom93](https://github.com/sachinsom93)
- Medium : [sachinsom507](https://medium.com/@sachinsom507)
- LinkedIn : [sachinsom507](https://www.linkedin.com/in/sachinsom507)

# Project Abstract

## [GSoC Project Page](http://LinikToYourGSoCProjectPage)

## [GSoC Project Proposal](http://LinikToYourGSoCProjectProposal)

## [GitHub Organization Repo](http://github.com/repo)

## [GitHub Personal Repo](http://github.com/repo)

## [Commits during GSoC 2017](http://github.com/commits)

## [Project Demo Video](http://LinkToDemoVideo)

## [Project Wiki](http://github.com)

## [GSoC Blog](http://GSoCBlog)

# Work Summary

# What Covered
**Week 1**
  * Designed and Implemented database architecture having   seperate modal classes for each entitiy i.e. `Admin`, `Extractor`, `Management`, `Cases` and `Tasks`.
  * Refactored flask backend structure of OpenMF.
  * Refactored existing APIs incorporating newly designed database architecture and flask structure.
  * **Related PR**
    * [week 1 commit]()

**Week 2**
  * Implemented Authentication routes using `JSON WEB TOKEN`.
  * Developed authentication login and signup process in frontend using authentication routes.
  * **Related PR**
    * [week 2 commit]()

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
     * [commit week 3]()

**Week 4**
  * Developed Entire Frontend Section for `Admin`
    * Components for listing, editing and deleting both kinds of members i.e extractor and management.
    * Implemented create and add new member components.
    * Developed frontend pages to see active cases and tasks assigned to members(completed and uncompleted tasks).
  * **Related PRs**
    * [commit week 4]()

**Week 5**
  * Created Frontend Section for `Management` member
    * Implemented some APIs related to `Management` member.
    * Developed Components for listing all extracted cases, rendering contents of a case directory in hierarchical manner etc.
  * **Related PRs**
    * [commit week 5]()

**Week 6**
  * Extending frontend section for `Management` member created in week 5.
  * Implemented routes for showing all the files of each case directories.
  * Developed frontend for the same integrating above created APIs.
  * **Related PRs**
    * [commit week 6]()

**Week 7**
  * Created Frontend Section for `Extractor` member.
  * Implemented Data Extraction part in Frontend by integrating data extraction API routes.
  * **Related PRs**
    * [commit week 7]()

**Week 8**
  * Performed Data Visualization for extracted data.
  * Created Bar, line, Polar etc charts for analysing browser history data.
  * **Related PRs**
    * [commit work 8]()

**Week 9**
  * Created REST APIs for verify email address and forgot password.
  * Developed Frontend and integrated this with APIs for verify address and forgot password.
  * Worked on some bugs related to `Admin` Section.
  * **Related PRs**
    * [commit work 9]()

**Week 10**
  * Updated Readme for Frontend and backend section of OpenMF.
  * Created Videos regarding installation-setup and demos of frontend and backend sections.
  * Worked on some left over bugs.
  * **Related PRs**
    * [commit week 10]()


# What left

#