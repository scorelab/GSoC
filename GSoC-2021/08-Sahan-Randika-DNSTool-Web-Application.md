# DNSTool-Web-Application

## Student Info

- Name - Sahan Randika
- Email - [shnrndk@gmail.com](mailto:shnrndk@gmail.com)
- GitHub Profile - [shnrndk](https://github.com/shnrndk)
- Medium - [@shnrndk](https://shnrndk.medium.com/)
- Twitter - [@shnrndk](https://twitter.com/shnrndk)

# Project Abstract
DNSTool-Frontend is the main access portal of the DNSTool which is designed to monitor the given set of internet resources like domains, IP, SOA, etc. Frontend allows users to upload their scanning seed list(s) and control the scans as well as schedule them. This project is to design a responsible and user-friendly single-page application as the frontend (dashboard).

Live demo - [https://dnsip.pages.dev/](https://dnsip.pages.dev/)

<kbd>
  <img src="https://user-images.githubusercontent.com/43110114/130364461-e363c231-292f-4fc9-b973-eefdfb2b10a6.png">
</kbd>



## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5463237421694976)

## [GSoC Project Proposal](https://drive.google.com/file/d/1iPjKnFnNijsDMghImMNgEfoqJhAKCaV9/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/DNSTool-Web-Application)

## [GitHub Personal Repo](https://github.com/shnrndk/DNSTool-Web-Application)

## [Commits during GSoC 2021](https://github.com/scorelab/DNSTool-Web-Application/commits/main)

## [Project Demo Video](https://youtu.be/nQgedVSq1Hs)

## [Project Wiki](https://github.com/scorelab/DNSTool-Web-Application/blob/main/README.md)

## [GSoC Blog](https://medium.com/scorelab/gsoc-2021-with-score-lab-da95b0686f29)

# Work Summary
Throughout the GSoC 2021 program, I implemented the DNSTool-Web-Application. In the first step of the coding phase, I started to communicate with mentors to get a proper initial plan of the DNSTool-Web-Application. 
Before moving on to the coding, first I've designed UI mockups using the Figma. Then I focused on the coding part of the UI mockups.
DNSTool-Web-Application is developed by React. React is the most popular front-end framework right now. For the state management, I used the Redux library. To implement with the React I used the react-redux library. I used the material-UI component library to develop UI components with React. It makes front-end development easier and faster. 
After the UI coding finished, I focused on connecting the backend APIs with the DNSTool-Web-Application. To make requests with the APIs, I've used the Axios library. I implemented the user login function using Google Firebase Authentication. I have implemented front-end authentication using the redux-auth-wrapper library. 
# What Covered
1. Designed the UI mockups using Figma
2. Initiated DNSTool-Web-Application using React frontend framework.
3. Implemented redux store using the redux state management library.
4. Implemented all UI mockups into react components using Material UI library.
5. Added user login using Google Firebase Authentication.
6. Implemented user registration. For the user registration I've implemented a password strength meter using zxcvbn library.
7. Added form validations(Email validation - Check if the email belong to accepted organisation domain and Correct Email Format) to the user registration.
8. Added Google reCAPTCHA v3 protection to the user registration.
9. Connected all the backend APIs with the frontend using the axios library and using the redux actions methods.
10. Implemented create scan functionality.
11. Implemented delete scan and update state of the scan functionalities.
12. Implemented the download key option in the frontend.
13. Implemented a material ui table to view the scans, filter and multi select the scans.
14. Implemented frontend authentication to add route guards to UI components using the redux-auth-wrapper library. 
15. Made the frontend responsive using Material UI media queries.

# What left
1. Create storybook components.

# References

1. [React](https://reactjs.org/)
2. [Redux](https://redux.js.org/)
3. [React-Redux](https://react-redux.js.org/)
4. [Firebase Authentication](https://firebase.google.com/docs/auth)
5. [Material-UI](https://next.material-ui.com/)
6. [Google reCAPTCHA v3](https://developers.google.com/recaptcha/docs/v3)
7. [zxcvbn](https://github.com/dropbox/zxcvbn)
8. [Axios](https://www.npmjs.com/package/axios)
9. [Redux Auth Wrapper](https://www.npmjs.com/package/redux-auth-wrapper)
10. [Figma](https://www.figma.com/)
11. [Storybook](https://storybook.js.org/)

