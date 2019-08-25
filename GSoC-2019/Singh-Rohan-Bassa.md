# Bassa - Shifting Bassa codebase from Angular to React

## Student Info
  * Name - Rohan Singh
  * Email - rohaniiitv@gmail.com
  * University - Indian Institute of Information Technology Vadodara
  * GitHub profile - https://github.com/singhrohan62
  * LinkedIn profile - https://www.linkedin.com/in/rohan-singh-015003154/

### Project Abstract
Bassa solves the problem of wasting internet bandwidth by queuing a download if it is larger than a given threshold value in high traffic and when the traffic is low, it completes the download of the files. Though the basic functionality of Bassa is complete and working, however AngularJS is not much supportive right now and since ReactJS is the new trending frontend library for building user interfaces, it is better to evolve with time and adopt new changes as **Change is Inevitable**.
Below is the list of tasks I completed for this project:

  * Enhance and fix Bassa User Interface
  * Provide Mobile support
  * Provide clean codebase to the repository
  * For enhancing User Interface, use Material UI, Redux Saga and React Router
  * Use React Boilerplate


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4739588881383424)

### [GSoC Project Proposal](https://docs.google.com/document/d/1NyjKDUtW6P5XD96WwCVZr_trpPAY3noAx_5_NcBi9AA/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/bassa)

### [GitHub Personal Repo](http://github.com/singhrohan62/bassa)

### [Commits during GSoC 2018](https://github.com/scorelab/Bassa/commits/develop?author=singhrohan62)

### [Project Demo Video](https://youtu.be/4FwCofupZvU)

### [Project Wiki](https://github.com/scorelab/Bassa/wiki)

### [GSoC Blog](https://docs.google.com/document/d/1_Kyn5pEUYYHcwkcdtGRVvRSMg6QxsNqDzOUi-th_lMo/edit?usp=sharing)

### Work Summary
I had wonderful experience during this summer because I got to learn new technologies and frameworks which I later 
 used in implementing the application. Below is the list of the pull requests I submitted during this summer:

* Base for the React application was created using Create React App. [](https://github.com/scorelab/Bassa/pull/780)
* Created static components which later was used in implementing Dashboard, Completed and Queued components under Storybook environment. [#780](https://github.com/scorelab/Bassa/pull/788)
* Completed static UI implementation by creating Admin and Login components too. Added snapshot tests and unit tests int the application. [#807](https://github.com/scorelab/Bassa/pull/807)
* Tested the API endpoints of Bassa API implemented authentication flow in the application. [#809](https://github.com/scorelab/Bassa/pull/809)
* Completed routing setup of the application with React router. [#812](https://github.com/scorelab/Bassa/pull/812)
* Completed setup of redux into the application. Added Formik for signup form validation and ESLint, Prettier as code linter and formatter following Airbnb style guide. [#817](https://github.com/scorelab/Bassa/pull/817)

### What Covered
1. Creating React application for Bassa.
2. Adding features provided by Angular UI into the new React application.
3. Providing clean codebase using linting and formatting tools.
4. Provided testing environment for new developers to test their changes.

### What left
1. Add end-to-end testing inside the application.
2. Integrate MinIO to the React application and use it.

### Reference
* React - https://reactjs.org, https://create-react-app.dev/docs/getting-started
* Storybook React - https://storybook.js.org/docs/guides/guide-react
* React Route - https://reacttraining.com/react-router/web/guides/quick-start
* Redux - https://redux.js.org, Redux Saga - https://redux-saga.js.org
* Jest - https://jestjs.io, Enzyme - https://airbnb.io/enzyme/