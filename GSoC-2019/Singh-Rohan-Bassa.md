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

* Base for the React application was created using Create React App. [#780](https://github.com/scorelab/Bassa/pull/780)
* Created static components which later was used in implementing Dashboard, Completed and Queued components under Storybook environment. [#788](https://github.com/scorelab/Bassa/pull/788)
* Completed static UI implementation by creating Admin and Login components too. Added snapshot tests and unit tests int the application. [#807](https://github.com/scorelab/Bassa/pull/807)
* Tested the API endpoints of Bassa API implemented authentication flow in the application. [#809](https://github.com/scorelab/Bassa/pull/809)
* Completed routing setup of the application with React router. [#812](https://github.com/scorelab/Bassa/pull/812)
* Completed setup of redux into the application. Added Formik for signup form validation and ESLint, Prettier as code linter and formatter following Airbnb style guide. [#817](https://github.com/scorelab/Bassa/pull/817)

### What Covered
1. **Creating React application for Bassa**.
  * I used Create-React-App for implementing the React application for Bassa. Since, it is preconfigured with tools like Webpack and Babel, there is no need to worry for downloading extra dependencies in the project for using JSX syntax or for creating development environment. Focus is on the code.
  * After the discussion with my mentor @agentmilindu and @charithccmc, we came to conclusion that I will be developing the components used in the React application in Storybook environment.
  * Storybook provides an isolated environment where developers can develop and create new components without messing with the actual working app and can create and test the response of the component on dummy data. Moreover, one can also simulate events in Storybook environment.

2. **Adding features provided by Angular UI into the new React application**.
  * To develop the components, which will be required by the Bassa application, I divided the whole application into five major components.
  * The first component is the *Login* component which will be rendered first whenever a user runs the application first time.
  * This component contains three child components.
  * One of them is used for logging into the application (*Appbar*), second one for signing in a first time visitor who wants to become a user (*UserSignup*) and a component telling the visitor about Bassa (*BassaIntroBox*).
  * For validation of the form being submitted by the first-time user, I used Formik for handling the form submission and data incoming. I used Yup as schema validator for validating data entered by the user.
  * After the user has logged into the application, *Dashboard* component renders on the screen. This component is used for adding link to the file the user wishes to download and it also displays the list of files which have been queued and downloaded.
  * It also contains links to the components *Completed* and *Queued* which are used to render the list of completed and queued downloads respectively.
  * The last component is for the users which are admins. The *Admin* component also consists of three child components.
  * The first one displays the pending signup requests (*PendingSignupRequests*) from different users which admin can approve. The second component allows the admin to start or kill downloading files (*StartKillDownloads*) and the last component displays the contributions of different users on the basis of size of the file they added (*UsageStats*).

  * After the components were built, I needed to connect them and provide routes to each parent component.
  For adding routes to the application, I used *React-Router*, a library frequently used in React applications for creating routes into the application.
  * I made sure that only *Login* component is a public route. For that, I encapsulated remaining components under a created PrivateRoute which would check if the user is logged in or not. If not, then it would redirect it to the *Login* component.
  * Also, I created a component (*NotFound404*) for user who enters an undefined route in the application to make him aware of his mistake and proceed to the right path for accessing the application.

  * After creating routes for the application, it was time to create a global unique state tree for the application which would be accessible and be modified from every corner of the application when required.
  * Hence, *Redux* was introduced into the application. It is a famous library very frequently used with React applications for creating a single state tree whose scope is throughout the application.
  * Since, requests were needed to be made to the Bassa server for accessing and manipulating the data,  *Redux Saga* was added to the application to handle API requests.
  * The state was divided into two major substates. One used for handling user data and the other for file data.

3. Providing clean codebase using linting and formatting tools.
  * For an application, it's good to follow a style guide and linting rules so that developers do not create and follow their own individual formatting styles.
  * I added *ESLint* as the linting tool into the application which would restrict other developers for following their own style guide and follow only the ESLint rules.
  * For formatting code, I added *Prettier* to the application for maintaining consistent style throughout the application.
  * I added *Airbnb* style guide into the application. I also added husky along with lint-staged and pretty-quick so that whenever a contributor wishes to commit his/her changes, he should see linting mistakes he/she did and resolve it later.

4. Provided testing environment for new developers to test their changes.
  * For testing the components, I used *Jest* which is test runner and assertion library (for asserting in tests) running in Node environment.
  * For snapshot testing, I used *Enzyme* which provides with methods like *shallow()* and *mount()*. I used the former one for functional components and latter one for the components which were wrapped under Higher Order Components.
  * The aim for testing the components was to check how the component responds to events occuring inside it.
  * I used *mock functions* a feature provided by Jest to check if a certain function was called or not.
  * To test if a certain function was called on any event occurence, I created mock function for them and simulated events with the help of DOM simulation to check if the function was called or not.

### What left
1. Add end-to-end testing inside the application.
  * Testing is an important part of the application which provides confidence to the developer.
  * Snapshot and unit tests testing the component via DOM simulation and mock functions have been done in the application. What we require now is to add end-to-end testing inside the application.

2. Integrate MinIO to the React application and use it.
  * Since, MinIO will be used as new file system for Bassa, it's better to accept and apply those changes in the application too.

### Reference
* React - https://reactjs.org 
* Create React App - https://create-react-app.dev/docs/getting-started
* Storybook React - https://storybook.js.org/docs/guides/guide-react
* React Route - https://reacttraining.com/react-router/web/guides/quick-start
* Redux - https://redux.js.org
* Redux Saga - https://redux-saga.js.org
* Jest - https://jestjs.io
* Enzyme - https://airbnb.io/enzyme
* ESLint - https://eslint.org
* Prettier - https://prettier.io/docs/en/index.html
* Airbnb React Style Guide - http://airbnb.io/javascript/react/