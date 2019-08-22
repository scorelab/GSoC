# Project Name

TrackPal

## Student Info

- <b>Name</b>: Shehan Dhaleesha
- <b>Email</b>: [shehandvid@gmail.com](mailto:shehandvid@gmail.com)
- <b>University</b>: University of Colombo School of Computing, Sri Lanka
- <b>GitHub Profile</b>: [https://github.com/shehand](https://github.com/shehand)
- <b>LinkedIn Profile</b>: [https://www.linkedin.com/in/shehandvid](https://www.linkedin.com/in/shehandvid)

### Project Abstract

In Sri Lanka, the transportation tracking problem is a huge challenge. The passengers can't determine the current position of their transportation medium (in this case it may be bus or train) correctly. So they have to wait until it arrives at their pickup location (it may be a bus stop, bus stand or railway station). So TrackPal is the solution to this problem. Trackpal is a public based mobile application which will help users to track their transportation medium.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5970850174468096)

### [GSoC Project Proposal](https://docs.google.com/document/d/184m5mgA4FLctAEl1wXBU8sU7pgaY-Je8BibP1VwDgQQ/edit?usp=sharing)

### GitHub Organization Repo

- [TrackPal Repo](https://github.com/scorelab/TrackPal) - Mobile application

### [GitHub Personal Repo](https://github.com/shehand/TrackPal)

### [Commits during GSoC 2019](https://github.com/scorelab/TrackPal/commits?author=shehand)

### [Project Demo Video](https://drive.google.com/open?id=10HCShntPdY99JS23T1mV3rTgBzv-KU5q)

### [Project Wiki](https://github.com/scorelab/TrackPal/wiki)

### GSoC Blog

- [Road To GSoC — 2019 with SCoRe Lab — Vol 1](https://medium.com/@sonodewcomplex/road-to-gsoc-2019-vol-1-ffb51adf73cc)
- [Road To GSoC — 2019 with SCoRe Lab — Vol 2](https://medium.com/@sonodewcomplex/road-to-gsoc-2019-with-score-lab-vol-2-9bc541d6ed5e)

### Work Summary

For the GSoC 2019, I've implemented the basic functionality of the moblie application. The application is implemented with react-native, so the apps for iOS and Android can be built at the same time. And unit testing for all the components in the mobile application have been done using jest.

### What Covered

In TrackPal v1.0.0 (stable)

 - Implemented SignIn / SignUp (Facebook/Google/Email-Password).
 - Implemented Navigation (Bottom Tab/Drawer Navigation).
 - Implemented Onboarding screens / Landing screen.
 - Implemented Shared Bus Details / Train Details screens.
 - Implemented View Shared Details screen (For every individual list item in shared bus details and shared train details screens).
 - Implemented Share Details screen (for both train and bus details. This screen is configured with google maps).
 - Configure Google Maps with the application using Google Maps API.
 - Configured firebase with the application.
 - Implemented searching mechanism based on the end point of a shared transportation details.
 - Implemented Forget password functionality by using firebase
 - Buid the Android applcation for a release.
 
### What left

 - The shared route of a transportation medium should be validated using proper route details.
 - iOS build for the appliation should be done.
 - Remove duplcate entries from the shared lists.
 
### Reference

1. React-Native Docs - http://facebook.github.io/react-native/
2. Google Map API - https://cloud.google.com/maps-platform/
3. Firebase Docs - https://firebase.google.com/