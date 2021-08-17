# LabelLab

## Student Info

- Name - Amlan Kumar Nandy
- Email - amlannandy5@gmail.com
- University - Trident Academy of Technology, Bhubaneshwar, India
- GitHub Profile - https://github.com/amlannandy
- Medium - https://amlannandy.medium.com/
- LinkedIn Profile - https://www.linkedin.com/in/amlan-nandy/

## Project Abstract

![labellab](https://user-images.githubusercontent.com/45410599/125047461-a1ebf100-e0bc-11eb-9849-0aa7eb15156c.png)

LabelLab is an image analysis and classification platform for machine learning (ML) researchers. Originally built to classify images of elephants, it has been developed over the years and is now a full-fledged ML utility tool that is able to classify all kinds of images and carry out a number of ML-related tasks in a project-based manner while teaming up with other researchers.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5444207780560896)

## [GSoC Project Proposal](https://drive.google.com/file/d/1lqfnTeeKTtqyiyQGvweSLRJVAJymrmrA/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/LabelLab)

## [GitHub Personal Repo](https://github.com/amlannandy/labellab)

## [Commits during GSoC 2021](https://github.com/scorelab/LabelLab/commits?author=amlannandy)

## [Project Wiki](https://github.com/scorelab/LabelLab/wiki)

## [GSoC Blog](https://amlannandy.medium.com/)

# Work Summary

LabelLab mainly consists of 3 sections -

1. Backend built using Flask
2. Frontend built using React.js
3. Mobile Application built using Flutter

Albeit a couple of features that were exclusive to the mobile application, most of my work across GSoC 2021 spanned across all 3 sections of the project.

## Expanding Team Management

- Now inside a project, the project admin can create multiple teams, each having a specific functionality, and add users to them.
- These teams can later be updated or deleted by an admin.
- These teams can only perform actions inside a project that are authorized by their role `(role-based access control)`. E.g. - A models team member can only work with models inside that project.
- The project owner can make other users admins for better project management. The admin priviledge can also be revoked by the owner when necessary.
- Project structure was modified to accomodate multiple admins.
- Admins form a superset of all other role and can perform any actions inside a project
- Now, a member can also voluntarily leave a project. Earlier, they had to removed by the admin.

<div style="flex-direction: row; margin-bottom: 60px;">
<img src='https://user-images.githubusercontent.com/45410599/122702581-525c9700-d26d-11eb-8a03-a5b755ab1855.jpg' height='400px' style="margin-right: 10px;" />
<img src='https://user-images.githubusercontent.com/45410599/126673118-2386ef2b-6680-4957-8558-8da86bf11032.gif' height='400px' />
</div>

### Related PRs -

- [#607 - [Backend] Improved Team Management](https://github.com/scorelab/LabelLab/pull/607)
- [#608 - [Mobile] Improved Team Management](https://github.com/scorelab/LabelLab/pull/608)
- [#613 - [Frontend] Improved Team Management](https://github.com/scorelab/LabelLab/pull/613)

## Implementing Project Activity Tracking

- Created a Project Activity Tracking System which helps keep track of all changes inside a project such as -
  - Adding/removing members
  - Adding and labelling images
  - Creating labels
  - Creating and training models
  - and much more...
- Each activity log is associated with a particular category (general, images, labels etc) and a particular user (the one who made that change).
- These activity logs can be filtered for analysis of the progress of the project.
  - `category-specific` - View activity logs of a particular category.
  - `member-specific` - View activity logs of a particular project member.
  - `team-specific` - View activity logs of a particular team.
  - `entity-specific` - View changes made to a particular entity (image, label, model etc)

<div style="flex-direction: row; margin-bottom: 60px;">
<img src='https://user-images.githubusercontent.com/45410599/129543416-dea760b6-eb3a-4f64-a275-4572b7ab308d.jpg' height='400px' style="margin-right: 10px;" />
<img src='https://user-images.githubusercontent.com/45410599/126866771-2584c384-142e-42ff-90f5-ba5f0f39ce0b.gif' height='400px' />
</div>

### Related PRs -

- [#604 - [Backend] Implemented Project Activity Tracking System](https://github.com/scorelab/LabelLab/pull/604)
- [#606 - [Mobile] Implemented Project Activity Tracking System](https://github.com/scorelab/LabelLab/pull/606)
- [#614 - [Frontend] Implemented Project Activity Tracking](https://github.com/scorelab/LabelLab/pull/614)

## Implementing Team-wise Chat System

- Built a Team-wise Chat System for team members to converse about project progress.
- Used web sockets (Socket.io) for maintaining a live feed of messages with minimal lag

<div style="flex-direction: row; margin-bottom: 60px;">
<img src='https://user-images.githubusercontent.com/45410599/129541842-95adaf0b-0572-4ea7-9fe1-ef177a257f0e.gif' height='400px' style="margin-right: 10px;" />
<img src='https://user-images.githubusercontent.com/45410599/128378626-0f37d041-9e8f-4d88-84a3-8fc7686ffcf2.gif' height='400px' />
</div>

### Related PRs -

- [#610 - Implemented Team-wise Chat System](https://github.com/scorelab/LabelLab/pull/610)
- [#615 - [Frontend] Implemented Team-wise Chat System](https://github.com/scorelab/LabelLab/pull/615)

## Migrating Mobile Application to Flutter 2.0

- Migrated the mobile application to Flutter 2.0 along with full support for null safety.
- Fixed dependency issues
- Upgraded all packages to their null-safe versions.
- Replaced packages which didn't support null safety with alternatives

### Related PRs -

- [#603 - Migrate to Flutter 2.0 and fix Dependency Versions](https://github.com/scorelab/LabelLab/pull/603)

## Creating a Backend Service Selection Utility

- Created a backend service selection utility in the mobile application.
- This allows the user to enter the URL of the LabelLab API instance that the application should use.
- This provides the functionality to connect to multiple backend instances without much tinkering.

<div style="flex-direction: row; margin-bottom: 60px;">
<img src='https://user-images.githubusercontent.com/45410599/129545745-7dc3e7af-f021-4cef-b5c5-3fa5da101e7c.jpg' height='400px' />
</div>

### Related PRs -

- [#605 - Implemented Backend Service Selection functionality in Mobile Application](https://github.com/scorelab/LabelLab/pull/605)

## Fixing Bugs in Mobile Application

- Fixed existing bugs present in the mobile application
- Implemented minor features that were missed earlier

### Related PRs -

- [#612 - Fixed bugs and implemented missed features](https://github.com/scorelab/LabelLab/pull/612)

## Writing Unit Tests

- Wrote unit tests for the mobile applications using Mockito.
- The tests covered all API endpoints that are being used by the mobile application.

### Related PRs -

- [#611 - [Mobile] Added tests for all used API Endpoints](https://github.com/scorelab/LabelLab/pull/611)

## Writing documentation in GitHub Wiki

- Originally, all of the project's documentation was present in a single readme.
- Moved that documentation to the Project Wiki.
- Also added documentaion for the new features that were implemented during GSoC '21.

### Related PRs -

- [#616 - Update Documentation](https://github.com/scorelab/LabelLab/pull/616)

# What Covered

- Migrated mobile application to Flutter 2.0 with null safety
- Created a backend service selection utility in mobile application
- Fixed bugs in mobile application
- Wrote unit tests for all endpoints used in mobile application
- Expanded team management in backend, frontend and mobile
- Implemented project activity tracking in backend, frontend and mobile
- Implemented a team-wise chat system in backend, frontend and mobile
- Wrote documentation for the entire project on Github Wiki

# What left

I managed to complete all my milestons within the coding period, and also implemented a few additional features. But there are a few other features the project could benefit from such as -

- Creating initialization scripts for the project
- Writing unit tests for the backend
- Fixing dependencey versions and warnings in the frontend

# Reference

- [Flutter documentation](https://flutter.dev/docs)
- [React.js documentation](https://reactjs.org/docs/getting-started.html)
- [Flask Documentation](https://flask.palletsprojects.com/en/2.0.x/)
- [Socket.io Documentation](https://socket.io/docs/v4/index.html)
- [Mockito Documentation](https://flutter.dev/docs/cookbook/testing/unit/mocking)
