# LabelLab

## Student Info

- Name - Nishant Andoriya
- Email - andoriyanishant@gmail.com
- University - Indian Institute of Information Technology, Vadodara
- GitHub Profile - https://github.com/M-A-D-A-R-A
- Medium - https://medium.com/@andoriyanishant
- LinkedIn Profile - https://www.linkedin.com/in/andoriya-nishant/

# Project Abstract

LabelLab is an image analysis and classification platform for machine learning (ML) researchers. Originally built to classify images of elephants, it has been developed over the years and is now a full-fledged ML utility tool that is able to classify all kinds of images and carry out a number of ML-related tasks in a project-based manner while teaming up with other researchers. It allows the user to upload images in bulk, label them and use image path tracking feature. Additionally, it supports automatic labeling of a set of unlabeled images by running classification across trained models.
## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/BRb6s0fz)

## [GSoC Project Proposal](https://docs.google.com/document/d/16-mgEN1X5-EVexpJx0HfPoCrolRXRCWzG3VfaAEdGBA/edit)

## [GitHub Organization Repo](https://github.com/scorelab/LabelLab)

## [GitHub Personal Repo](https://github.com/M-A-D-A-R-A/LabelLab)

## [Commits during GSoC 2022](https://github.com/scorelab/LabelLab/commits?author=M-A-D-A-R-A)
## [Project Wiki](https://github.com/scorelab/LabelLab/wiki)

## [GSoC Blog](https://m-a-d-a-r-a.github.io/blog.html)

# Work Summary
The codebase architecture involves three components :
1. Backend - RESTful Flask API
2. Frontend - ReactJs application
3. Mobile - Flutter application

For GSoC 2022, the main objectives were to improve the project
management and version tracking system to make it more collaborative. My work spanned mainly across Backend and Mobile App

## Created an Issue Tracking System

- A project member can now create issues within a project.
- An issue must necessarily include a title, description and category.
- These issues can later be updated or deleted by project members.
- The project members can view the list of all issues within a project and filter them based on category, priority etc.
- Worked on creating [Figma](https://www.figma.com/file/0DMmXmG6OW2JaZgZwGU2DL/LabelLab?node-id=0%3A1) designs for ```issue Detail Screen``` and `Issue Tile` Components
- Comment section improves the project management and make it more collaborative by allowing project members to discuss a particular issue and its updates.

<div style={display: flex;}>
        <img src='https://user-images.githubusercontent.com/56160262/189531716-3f9bbc68-2442-4d4b-a303-1e9c767a1d07.gif' height='450px' style={margin-right:10px;} />
    <img src='https://user-images.githubusercontent.com/56160262/189531181-e03028ed-074b-40a3-8aee-a023d82fc33e.gif' height='450px' style={margin-right:10px;} />
    <img src='https://user-images.githubusercontent.com/56160262/189531542-0f670ad5-02f8-451f-975e-da92ce0d374c.gif' height='450px' style={margin-right:10px;} />
</div>

### Related PRs -

| PR Link   | Description    |  Issue Link     |
|-----------|----------------|-----------------|
| [#638](https://github.com/scorelab/LabelLab/pull/638) | Merged ✅ |  [Backend] Initialize Issues Controller   |
| [#640](https://github.com/scorelab/LabelLab/pull/640) | Merged ✅ | [Backend] Initialize Comment Controller |
| [#644](https://github.com/scorelab/LabelLab/pull/644) | Merged ✅ | [Backend] Implement Listing Issues Endpoints
| [#645](https://github.com/scorelab/LabelLab/pull/645) | Merged ✅ | [Backend] Implement Endpoint for Add Comment 
| [#648](https://github.com/scorelab/LabelLab/pull/648) | Merged ✅ | [Backend] Implement Endpoint for listing all comments in an issue
| [#658](https://github.com/scorelab/LabelLab/pull/658) | Merged ✅ | [Mobile] Implement the screens for displaying all issues
| [#666](https://github.com/scorelab/LabelLab/pull/666) | Merged ✅ | [Mobile] Issue List TIle UI
| [#669](https://github.com/scorelab/LabelLab/pull/669) | Merged ✅ | [Mobile] Issue detail screen and Comment Feature

## Flutter CI/CD WorkFlow

Using Github Action, implemented CI/CD flutter workflow that would run on all new PR, every subsequent push to a PR, as well as on the main repo. This would enforce strict quality control and reduce human error, which will be immensely helpful in the long term as we integrate more tests.
### Related PRs -
| PR Link   | Description    |  Issue Link     |
|-----------|----------------|-----------------|
| [#653](https://github.com/scorelab/LabelLab/pull/653) | Merged ✅ |  [Mobile] Flutter CI workflow (Fixes [#627](https://github.com/scorelab/LabelLab/issues/627))

## Migrating Mobile Application to Flutter 3.0
 - Migrated the mobile application to Flutter 3.0 
 - Fixed dependency issues
 - Restored App theme
### Related PRs -
| PR Link   | Description    |  Issue Link     |
|-----------|----------------|-----------------|
| [#649](https://github.com/scorelab/LabelLab/pull/649) | Merged ✅ |  [Mobile] flutter version upgrade to 3.0 (Fixes [#628](https://github.com/scorelab/LabelLab/issues/628))
| [#655](https://github.com/scorelab/LabelLab/pull/655) | Merged ✅ |  [Mobile] Restoring the App Theme

## Improved Chat System
 - Added the feature that allows user to tag/mention the following in chat 
    - Another project member - By typing `@`
    - Used `flutter_mention` package to unable user mentioning feature.
    - Improved the UI.

<img src='https://user-images.githubusercontent.com/56160262/189530603-28ffe42e-b73d-4f7c-bf07-561967460d98.gif' height='450px' style={margin-right:10px;} />

### Related PRs -
| PR Link   | Description    |  Issue Link     |
|-----------|----------------|-----------------|
| [#672](https://github.com/scorelab/LabelLab/pull/672) | Merged ✅ |  [Mobile] Tag user in comments

## Wrote unit and widget test
 - Added unit tests for Issue and comment API endpoints 
 - Added Widget test for Issue UI Components
### Related PRs -
| PR Link   | Description    |  Issue Link     |
|-----------|----------------|-----------------|
| [#670](https://github.com/scorelab/LabelLab/pull/670) | Merged ✅ |  [Mobile] API Test For Mobile
| [#674](https://github.com/scorelab/LabelLab/pull/674) | Merged ✅ |  [Mobile] widget test for Create issue screen

## Documentation

- Rectified database creation and virtual environment activation commands in documentation.
- Added documentation of Issue tracking system and Comments Features in Mobile Wiki.
# What Covered

- Created an issue tracking system in project
- Restructured the pre-existing project activity tracking system.
- Improved Chat System.
- Setup CI/CD WorkFlow 
- Migrated mobile application to Flutter 3.0 
- Restored the App theme
- Designed UI Commponent for the issue tracking system
- Wrote unit and widget tests

# What left
I implemented all the core milestones that I proposed, within the coding period. Some additional features/bug which are left and might prove useful for the project are -
- In the current tag user functionailty , once we post the commment, the UI dont reload itself.(Related issue [#673](https://github.com/scorelab/LabelLab/issues/673))
- In Comment Section , We can more features like `#` to Tag `Logs` and `Issues` the log id and issue id.
- Intigrate the notification and emailing system in mobile application.
- In Mobile application we can also have an Project Analytics and Report generation fetaure

# Reference
- [Flask Documentation](https://flask.palletsprojects.com/en/2.0.x/)
-  [Flutter documentation](https://flutter.dev/docs)
- [Mockito Documentation](https://flutter.dev/docs/cookbook/testing/unit/mocking)