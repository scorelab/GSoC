# CodeLabz

## Student Info

- Name - Nipuna Weerasekara
- Email - w.nipuna@gmail.com
- GitHub Profile - https://github.com/Niweera
- Medium - https://medium.com/@niweera
- Twitter - [@Niweera](https://twitter.com/Niweera)

### Project Abstract

CodeLabz is a platform where the users can engage with online tutorials and the organizations can create tutorials for the users. The platform is developed using ReactJS front end library and the back end is developed using the Google Cloud Firestore and Google Firebase Real-Time database.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5484930299068416)

### [GSoC Project Proposal](https://drive.google.com/file/d/1-DgbUlaMCgA7Tt9DmPrBLqfO7HWGw6vR/view)

### [GitHub Organization Repo](https://github.com/scorelab/Codelabz)

### [GitHub Personal Repo](https://github.com/Niweera/Codelabz)

### [Commits during GSoC 2020](https://github.com/scorelab/Codelabz/commits?author=Niweera)

### [Project Demo Video](https://youtu.be/-eD-lgZkKbI)

### GSoC Blog

- [GSoC 2020 with SCoRe Lab](https://medium.com/scorelab/gsoc-2020-with-score-lab-b43d208869c1)
- [GSoC 2020 with SCoRe Lab — Week 1](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-1-65a132110ed7)
- [GSoC 2020 with SCoRe Lab — Week 2](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-2-b6b2e0fedbf6)
- [GSoC 2020 with SCoRe Lab — Week 3](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-3-c74bdeab6bf9)
- [GSoC 2020 with SCoRe Lab — Week 4](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-4-975212da68b3)
- [GSoC 2020 with SCoRe Lab — Week 5](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-5-ca6f4962f14)
- [GSoC 2020 with SCoRe Lab — Week 6](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-6-6f97c5b8d470)
- [GSoC 2020 with SCoRe Lab — Week 7](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-7-754e5549d2d8)
- [GSoC 2020 with SCoRe Lab — Week 8](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-8-950e2dc95e56)
- [GSoC 2020 with SCoRe Lab — Week 9](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-9-b449b655315c)
- [GSoC 2020 with SCoRe Lab — Week 10](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-10-5e9816455b6)
- [GSoC 2020 with SCoRe Lab — Week 11](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-11-dbdf5dba23ad)
- [GSoC 2020 with SCoRe Lab — Week 12](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-12-b517cabb68c)
- [GSoC 2020 with SCoRe Lab — Week 13](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-13-72c67771c269)
- [GSoC 2020 with SCoRe Lab — Week 14](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-14-f2fb84a4cab0)
- [GSoC 2020 with SCoRe Lab — Week 15](https://medium.com/scorelab/gsoc-2020-with-score-lab-week-15-9c0ffda49655)

### Work Summary

Over the course of GSoC 2020, I implemented the backend functionalities in CodeLabz platform. The CodeLabz platform is developed using ReactJS and Ant Design UI framework. I created the schema for the CodeLabz platform databases using Google Firebase Realtime Database and Google Cloud Firestore. Also, I implemented the global state container using Redux alongside with React-Redux and React-Redux-Firebase. I also implemented the email sending functionality (for use cases such as, password reset, welcome email, etc.) with Cloud functions for Firebase. In addition, I implemented the push notifications service for CodeLabz platform using Cloud Functions for Firebase and Firebase Cloud Messaging. Moreover, I created the GitHub actions workflow to automatically deploy the CodeLabz platform to the Firebase Hosting platform upon a successful merge in the main repository. Finally, I added UI testing cases using Cypress testing framework.

### What Covered

1. Initiated the CodeLabz project with ReactJS and Ant Design with the Firebase RTDB and Firestore as the backend.
2. Implemented route protection for the React application.
3. Implemented the cloud functions for email sending using Cloud Functions for Firebase and Firestore Email Trigger extension.
4. Implemented social login functions with React-Redux-Firebase.
5. Implemented push notification sending feature with Firebase Cloud Messaging.
6. Created the GitHub action workflow for auto-deploy to Firebase hosting platform.
7. Implemented the global state container using Redux, React-Redux, React-Redux-Firebase and Redux-Firestore.
8. Added Firestore and Firebase database rules.
9. Implemented the database periodic maintenance using Google Cloud Pub/Sub and Cloud Functions for Firebase.
10. Implemented file upload to Cloud Storage for Firebase using React-Redux-Firebase.
11. Implemented client-side full-text search using elasticlunr.
12. Added Cypress test cases for UI automation testing.

### What left

1. UI/UX improvements
2. Add new push notification features

### Reference

1. [ReactJS](https://reactjs.org/docs/getting-started.html)
2. [Ant Design](https://ant.design/docs/react/introduce)
3. [Firebase Realtime Database](https://firebase.google.com/docs/web/setup)
4. [Cloud Firestore](https://firebase.google.com/docs/firestore)
5. [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging)
6. [Elasticlunr](http://elasticlunr.com/docs/index.html)
7. [Cloud Functions for Firebase](https://firebase.google.com/docs/functions)
8. [Cloud Storage](https://firebase.google.com/docs/storage)
9. [Cloud Pub/Sub Trigger](https://firebase.google.com/docs/functions/pubsub-events)
10. [Trigger Email Extention for Firestore](https://firebase.google.com/products/extensions/firestore-send-email)
11. [ReduxJS](https://redux.js.org/introduction/getting-started)
12. [React-Redux-Firebase](http://react-redux-firebase.com/)
13. [Redux-Firestore](https://github.com/prescottprue/redux-firestore)
14. [Cypress Test Framework](https://docs.cypress.io/guides/overview/why-cypress.html#In-a-nutshell)
15. [CodeLabz Live Demo](https://dev.codelabz.io/)
