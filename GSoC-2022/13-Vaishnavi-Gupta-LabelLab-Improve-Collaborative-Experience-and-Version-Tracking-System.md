# LabelLab

## Student Info

- Name - Vaishnavi Gupta
- Email - vaishnavigup1892@gmail.com
- University - Indian Institute of Technology, Roorkee
- GitHub Profile - https://github.com/vaishnavi-gupta18
- Medium - https://medium.com/@vaishnavigup1892
- LinkedIn Profile - https://www.linkedin.com/in/vaishnavi-gupta-02b208216/

# Project Abstract

![labellab](https://user-images.githubusercontent.com/45410599/125047461-a1ebf100-e0bc-11eb-9849-0aa7eb15156c.png)

LabelLab is an image analysis and classification platform for machine learning (ML) researchers. Originally built to classify images of elephants, it has been developed over the years and is now a full-fledged ML utility tool that is able to classify all kinds of images and carry out a number of ML-related tasks in a project-based manner while teaming up with other researchers. It allows the user to upload images in bulk, label them and use image path tracking feature. Additionally, it supports automatic labeling of a set of unlabeled images by running classification across trained models.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/VbS59H79)

## [GSoC Project Proposal](https://drive.google.com/file/d/1tXZzHNYMem-9l_DakXhze7D-WqpxsoV_/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/LabelLab)

## [GitHub Personal Repo](https://github.com/vaishnavi-gupta18/LabelLab)

## [Commits during GSoC 2022](https://github.com/scorelab/LabelLab/commits?author=vaishnavi-gupta18)

## [Project Wiki](https://github.com/scorelab/LabelLab/wiki)

# Work Summary

The codebase architecture involves three components :
1. Backend - RESTful Flask API
2. Frontend - ReactJs application
3. Mobile - Flutter application

For GSoC 2022, the main objectives were to improve the project
management and version tracking system to make it more collaborative. My work spanned mainly across Backend and Frontend.

## Created an Issue Tracking System

- A project member can now create issues within a project.
- An issue must necessarily include a title, description and category. The reporter can optionally add a due-date, priority level, its current progress status or associate it with an entity (such as image, label, model or an another issue).
- An issue can further be assigned to a team or specifically to a team member by the project admin (implementing `role-based access control`).
- These issues can later be updated or deleted by project members.
- The project members can view the list of all issues within a project and filter them based on category, team or a particular entity. 
- A detailed view of every issue with associated activity logs and comment section is provided. 
- Comment section improves the project management and make it more collaborative by allowing project members to discuss a particular issue and its updates.

![issue-listing](https://user-images.githubusercontent.com/76858666/189518312-f4d040f9-e803-48b1-8a74-4a9ae2ffec33.gif)

![issue details (fast)](https://user-images.githubusercontent.com/76858666/189518528-8cc229b9-8a69-4853-8b8d-9b80c027060f.gif)

### Related PRs -

- [#637 - [Backend] Add Issue and Comment models](https://github.com/scorelab/LabelLab/pull/637)
- [#639 - [Backend] Added 'Create issue' endpoint ](https://github.com/scorelab/LabelLab/pull/639)
- [#641 - [Backend] Implement Single Issues Endpoints (GET, PUT, DELETE)](https://github.com/scorelab/LabelLab/pull/641)
- [#647 - [Backend] Implement Endpoints for Single Comment (GET, PUT, DELETE)](https://github.com/scorelab/LabelLab/pull/647)
- [#650 - [Backend] Add pagination in issues](https://github.com/scorelab/LabelLab/pull/650)
- [#651 - [Backend] Add websocket for comments](https://github.com/scorelab/LabelLab/pull/651)
- [#654 - [Frontend] Implement the issues listing screen](https://github.com/scorelab/LabelLab/pull/654)
- [#656 - [Frontend] Implement issue detail screen](https://github.com/scorelab/LabelLab/pull/656)

## Restructured the pre-existing project activity tracking system

- Modified logging middleware to add logging functionality for following issue endpoints.
  - Create issue
  - Update issue
  - Delete issue
  - Assign Issue
- Allow tracking activity of a particular issue from issue listing screen and issue details screen.

![activity](https://user-images.githubusercontent.com/76858666/189518187-ca361607-df8d-4704-8b01-32d2313fd488.gif)

### Related PRs -

- [#643 - Modify logging middleware to handle issue controller endpoints](https://github.com/scorelab/LabelLab/pull/643)

## Improved Chat System

- Added the feature that allows user to tag/mention the following in chat :
    - Another project member - By typing `@`
    - Activity log - From a list of logs. Tagged using `#` with the log id
    - Issue - From a list of issues. Tagged using `#` with the issue id
- Used react-mentions package to unable user mentioning feature.
- Improved the UI.

![chat system](https://user-images.githubusercontent.com/76858666/189517993-e2b7c170-689a-43e0-9037-d47ce18849bc.gif)

### Related PRs -

- [#657 - [Backend + Frontend] Modify message model to include tagged entity](https://github.com/scorelab/LabelLab/pull/657)
- [#659 - [Backend + Frontend] Add user mentioning feature](https://github.com/scorelab/LabelLab/pull/659)

## Built a real-time Notification and Emailing system

- Added notifications and emailing system for following events :
    - Addition/Removal of project member
    - Addition/Removal of team member
    - Admin status
    - Issue is assigned to user
    - Assigned issue is updated
    - Comments on assigned issue
    - Mentioned/Tagged in chat
- User will recieve toast notifications on above events. Also, all the notifications can be found in the notifications button in navigation bar.
- Added emailing system to notify users of the above events.

![notification chat](https://user-images.githubusercontent.com/76858666/189517648-974eed8e-ece5-47e3-9c72-aabf4e9eae7e.gif)
![email](https://user-images.githubusercontent.com/76858666/189420123-57a46517-b488-4799-a4bb-bf51aada7972.png)

### Related PRs -

- [#662 - Add notification system backend](https://github.com/scorelab/LabelLab/pull/662)
- [#663 - Add notification system in frontend](https://github.com/scorelab/LabelLab/pull/663)
- [#664 - Add emailing system](https://github.com/scorelab/LabelLab/pull/664)

## Improved Project Analytics Page

- Added analytics for issues in the form of doughnut charts showing the number of issues classified according to category, status and priority.
- Fixed Label proportions chart.

![analytics short](https://user-images.githubusercontent.com/76858666/189517727-005280db-1d66-453d-bba1-0ccd5bea95cf.gif)

### Related PRs -

- [#665 - Implement issue analytics and fixed Label Counts analytics](https://github.com/scorelab/LabelLab/pull/665)

## Wrote unit tests for backend and frontend

- Add unit tests for Issue and comment API endpoints in backend.
- Added unit tests for Issue tracking system in frontend using enzyme.

### Related PRs -

- [#660 - Add unit tests for Issue and Comment Endpoints](https://github.com/scorelab/LabelLab/pull/660)
- [#671 - Add frontend tests in enzyme](https://github.com/scorelab/LabelLab/pull/671)

## Improved Error handling

- Added custom 401 (Unauthorized) on pages not accessible with user permissions.
- Added 404 (Not found) error page for non-existing urls.

<div style="flex-direction: row; margin-bottom: 60px;">
<img src='https://user-images.githubusercontent.com/76858666/189420665-f18d0afc-63b7-45e9-8102-d265419aa0f5.png' height='230px' style="margin-right: 10px;" />
<img src='https://user-images.githubusercontent.com/76858666/189420769-1603459a-a022-4619-b82a-127c6f24735f.png' height='230px' />
</div>

### Related PRs -

- [#668 - Add custom 404 and 401 error pages](https://github.com/scorelab/LabelLab/pull/668)

## Fix package dependency version

- Fixed package compatibility of Flask Socket-io and Client socket-io. 

### Related PRs -

- [#667 - Fix websockets ( Convert connection to polling)](https://github.com/scorelab/LabelLab/pull/667)

## Documentation

- Rectified database creation and virtual environment activation commands in documentation.
- Added documentation of Issue tracking system, notifications and emailing system. Updated documentation of Chat system and analytics.

# What Covered
- Created an issue tracking system in project
- Restructured the pre-existing project activity tracking system.
- Improved Chat System.
- Built a real time notification and emailing system.
- Improved Project Analytics Page.
- Wrote unit tests for the backend and frontend.
- Improved error handling.
- Upgraded Flask and npm packages to fix compatibility issues.

# What left
I implemented all the core milestones that I proposed, within the coding period. Some additional features which are left and might prove useful for the project are -
- Improve responsiveness
- Custom report generation
- Move the documentation to readthedocs

# References

- [React.js documentation](https://reactjs.org/docs/getting-started.html)
- [Flask Documentation](https://flask.palletsprojects.com/en/2.0.x/)
- [Socket.io Documentation](https://socket.io/docs/v4/index.html)
- [Sendinblue Documentation](https://developers.sendinblue.com/reference/sendtransacemail)
