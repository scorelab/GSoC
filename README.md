# GSoC
SCoRe Lab GSoC  Final Reports
Progress that was being made in the GSoC 2020 by different students:-

## Name - Aditya Bhatnagar
### What Covered

<br/>
<div align="center">
<br/>

![image-cropper](https://user-images.githubusercontent.com/43586052/88231334-ad6ac000-cc91-11ea-997a-fdc5539a1dad.png)
<br/>

![image-cropper](https://user-images.githubusercontent.com/43586052/88231351-b3f93780-cc91-11ea-98fb-161f8807b1ba.png)
<br/>

![team-dashboard](https://user-images.githubusercontent.com/43586052/89099631-69548980-d40e-11ea-84f1-079175e1b95d.png)
<br/>

![roles](https://user-images.githubusercontent.com/43586052/91656048-1cc6a180-ead3-11ea-9e0e-6b9b39d44bf6.png)
</div>
<br/>

- [x] Implement the functions to convert data to be displayed as statistical diagrams.
- [x] Write Analytics and Classification routes.
- [x] Revamp the whole frontend to work with the new backend including the major revamping in the way the labeller works.
- [x] Complete making the Image formatting/editing tool.
- [x] Fix image uploading for allowing meta data of images to remain intact so that the geolocation coordinates dont get lost.
- [x] Implement the Team feature inside the projects. Including the changes needed to the frontend which will allow formation of multiple teams with different or same team members and implement the teams dashboard.
- [x] Add role based project management and different roles cannot use different parts of the projects and admin role is assigned to the project creator.
- [x] Complete the tests for the code base.

### Milestone 3-

<br/>
<div align="center">
<br/>

![backend-tests](https://user-images.githubusercontent.com/43586052/90770452-6fec6780-e30f-11ea-8100-8ee28c005e75.png)
<br/>

![path-tracking-feature](https://user-images.githubusercontent.com/43586052/87033792-7f529e00-c204-11ea-95b2-90233985fdec.png)
<br/>

![path-tracking-feature](https://user-images.githubusercontent.com/43586052/87772052-d37e0380-c83e-11ea-9f5c-30cb8edba490.png)
<br/>

![path-tracking](https://user-images.githubusercontent.com/43586052/91656012-cd807100-ead2-11ea-80e3-4e14cb224404.png)
<br/>

![path-tracking-2](https://user-images.githubusercontent.com/43586052/91656015-cfe2cb00-ead2-11ea-8aaf-90ba4490a459.png)
</div>
<br/>

- [x] Implement Path-racking feature and allowing all/multiple images of the project to be used at once and trace the object.
- [x] Marking of latitudes and longitudes extracted from the image's metadata with Polylines feature of Google maps and custiomize it to meet the needs of the project.
- [x] Dockerize the LabelLab Flask server edit the existing docker-compose file for the frontend changes.
- [x] Prepare to Deploy the containerized app to GCP.
- [x] Adding additional commands for running tests and test coverage, cleaing the project of the .pycache files, showing all the urls ofthe project and upgrading the db and ading additional configs for travis production and testing.
- [x] Integrating the two builds of python 3.7 and 3.8 and test cases with Travis.
- [x] Implementation of the shpinx documentation.
- [x] Fix bugs and polish the new features and review the documentation.
- [x] Add pre-commit hooks for automatic code formatting before pushing the code.

### What left
- Full deployment of the already dockerized and deployement ready app.
- Completion of some parts of the Sphinx documentation.

## Name - Asitha Indrajith
### What Covered
* Designed a secure and structured database.
* Developed a secure authentication system.
* Adding, Commenting, liking, sharing and reporting word meanings.
### What left
* Full-text search with ElasticSearch or Algolia
* Pagination in some pages

## Name - D.DE SILVA
### What Covered
* Create develop interactive and attractive user-interface
* Add user management module
* Improve current crawler progress monitoring system
### What left
* Documentation need to be updated.
* Code need to be optimize more. 
* Complete more of the testing for the project.

## Name - Devon Wijesinghe
### Whats Covered
- Created Base Webiu Project
- Configured Costumizable theme and style variables file
- Implementated Baic Layout components which are reusable (eg: Header, NavBar and Footer Component)
- Implementated reusable Medium Feed Rendering component
- Implementated reusable Project List Rendering component
- Implementated reusable Publications List Rendering component
- Implementated reusable component to extract and render a public google mailing list
- Implementated reusable component which uses the Gitter API to extract and render the list of Gitter Rooms for a given Organziation
- Implemented a reusable SEO component which will optimize a sites online visibility
- Documentation on the reusable components
- Created Score Labs Site using Webiu Component
- Migrated ScoreLabs Site Markdown Data to new Site
- Created Leopard Labs Site using Webiu Component
- Implementated GRAPHQL quries to extract data from Markdown files
- Create custom page genration script to create project detail pages for each Score Labs / Leopard Labs project
### Whats left
The following are the tasks I could not not complete within the GSOC period:
- Implementation of Github Timeline Component
- Implementation of Github Org Member List Component
- Creation and Publising a NPM package for Webiu

## Name - Dilum De Silva
### What Covered
- Designed and finalized the ImageLab architecture.
- Developed the base UI of the ImageLab.
- Integration of maven build automation and dependency management for the project.
- Base architecture of the ImageLab based on MVC which consists,
    - Operators panel and functionalities.
    - Visualizing panel or the playground and functionalities.
    - Information panel and functionalities.
    - Preview panel and functionalities.
    - Properties panel and functionalities.
- Extendable architecture to add more operators.
- Validation mechanism to validate openCV operation order.
- Operator execution mechanism.
- Custom drag, drop and detect mechanism related to project requirements.
- Dashboard related functionalities (Refresh, Execute).
- OpenCV operations based operators,
    - Basic operators.
    - Geometric transformation operators.
    - Image conversion operators.
    - Image blurring operators.
- Reusable utility functionalities.
- Exporting openCV operation order as a file.
- Integration of lint issue checking to improve code quality.
- Code commenting.
- [Documentation](https://dilum1995.github.io/ImageLab/) as a jekyll website.   
### What left
- Introducing more openCV operations.
- Operator custom shape and animated attachable features.
- Testing related to the implementation.
- Exporting openCV operation order as an illustration.

## Name - Hansika Wanniarachchi
### What Covered
- Implemented webhook listner
- Implemented ukiyo push manager which involved with webhook configuration
- Implemented docker image puller and exsting image remover
- Implemented the deployment time scheduler
- Implemented ukiyo REST API
- Implemented container manager feature
- Created ukiyo-agent as a lightweight docker image
- Added test cases and feature validation
- Documentation - ukiyo wiki
- Added GitHub Actions
### What left
- Implementation of ukiyo dashboard
- Complete more of the testing for the project
- Implement the scheduler feature that will be configured for all the time zones

## Name - Harshit Verma
### What Covered
* [Added Unix support](https://github.com/leopardslab/expressPython/pull/8)
* [Fixed Jedi autocomplete](https://github.com/leopardslab/expressPython/pull/9)
* [Added expressPython gitter link](https://github.com/leopardslab/expressPython/pull/12)
* [Terminal Integration](https://github.com/leopardslab/expressPython/pull/13)
* [Added ANTLR Syntax highlighting](https://github.com/leopardslab/expressPython/pull/17)
* [Port QMake to CMake](https://github.com/leopardslab/expressPython/pull/19)
* [Ubuntu CI and deb package generation](https://github.com/leopardslab/expressPython/pull/25)
* [Doc update](https://github.com/leopardslab/expressPython/pull/26)
* [Ubuntu CI Artifacts Release feature](https://github.com/leopardslab/expressPython/pull/28)
* [Snippet, Tutorial and Notes Toggle button](https://github.com/leopardslab/expressPython/pull/29) *(Not part of proposal)*
* [Shortcut Keys feature](https://github.com/leopardslab/expressPython/pull/30) *(Not part of proposal)*
* [Issue and Bug templates](https://github.com/leopardslab/expressPython/pull/31) *(Not part of proposal)*
### What left
* macOs CI *(Work in progess) (Not part of proposal)*
* Windows CI *(Not part of proposal)*

## Name - Heshan Geasman
### What Covered
* Installation script generator
* Continuous Integration and Continuous Deployment
* Package-manager hints in cURL queries
* LogDude Bash logging micro framework
* GatsbyJS site base
* reated TOML files for existing installers
### What left
* Adding testing for existing installers, as this need some more standardizing as per mentors and got deprioritized.
* Complete the GatsbyJS site ( was not in the original plan ).

## Name - Shashindra
### What Covered
* Well-structured project design for High Maintainability and Readability of the Test Scripts
* WebDriver connection functions implementation
* Defining a Web page and its elements to a one class 
* External element object file (XML)
* Separate Test level to write test cases
### What left
* Cover more tests
* Code optimization
* Documentation

## Name - Lakindu Akash
### What Covered
- Implemeted creating and automating the VPN server
- Added certificate and token based authentication for clients
- Add client configuration scripts for Ubuntu and Android
- Implement the API for controling client access to the VPN server
- Dockerized the API
- [Documentation (Wiki)](https://github.com/bug-zero/bugzero-gateway/wiki)
### What left
- Filtering VPN logs by users and other critarias

## Name - Lakshyajeet Dwivedee
### What Covered
* Model management dashboard for adding, editing, deleting models
* Sub-module for choosing labels to train on
* Sub-module for choose image augmentation steps
* Sub-module for training custom model
* Sub-module for transfer learning
* Sub-module for training an uploaded model
* Sub-module for showing training accuracy and loss
* Sub-module for testing a trained model
* Sub-module for exporting a trained model in SavedModel, h5, and ONNX format
### What left
* Adding tests

## Name - Madhuri
### What Covered
Using scrapy-splash library intigreat splash to Tor Scraper scrapy crawler.
* Implement slash parser
* Store parse data in mariadb and elasticsearch
* Design and Implement Flask API expose data to front-end
* Design Analysis interface
* Implement Tree based structure using ETE Toolkit
### What left
* Unit testing need to be completed
* Integrated testing need to be completed
* Documentation needs to be updated

## Name - Mehant Kammakomati
### What Covered
* Fixed type errors and added logging to MySQL operations. Fixed multi-threading issue, compression feature and other related bugs. [`PR-1`](https://github.com/scorelab/Bassa/pull/918)
* Fixed Travis pipeline. [`PR-1`](https://github.com/scorelab/Bassa/pull/921)
* K8s scripts for monitoring and alerting system using Prometheus and Grafana dashboards. [`PR-1`](https://github.com/scorelab/Bassa/pull/925)
* Get Bassa Backend URL from env, made a workaround for now. [`PR-1`](https://github.com/scorelab/Bassa/pull/927)
* Written Python Client Library with retry, timeout and rate-limiting features. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/1) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/3)
* Added unittests, documentation, run bassa for tests and GitHub actions pipeline for tests and push to PyPi. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/4) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/5) | [`PR-3`](https://github.com/scorelab/bassa-client-libraries/pull/9) | [`PR-4`](https://github.com/scorelab/bassa-client-libraries/pull/11) | [`PR-5`](https://github.com/scorelab/bassa-client-libraries/pull/13) | [`PR-6`](https://github.com/scorelab/bassa-client-libraries/pull/16) | [`PR-7`](https://github.com/scorelab/bassa-client-libraries/pull/20) | [`PR-8`](https://github.com/scorelab/bassa-client-libraries/pull/22)
* Add Golang Client library with timeout, retry and rate-limiting features. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/25)
* Add mandatory artifacts and services for the new GitHub repository - Bassa Client Libraries. 
[`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/6) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/17) | [`PR-3`](https://github.com/scorelab/bassa-client-libraries/pull/18) | [`PR-4`](https://github.com/scorelab/bassa-client-libraries/pull/19) | [`PR-5`](https://github.com/scorelab/bassa-client-libraries/pull/21)
### What left
* Make Bassa v1.0 deployment - *not strictly part of the proposal*
* Review security layers for Bassa server and add any needed patches - *not part of the proposal*

## Name - Nimesha
### What Covered
* Smart contract project for a hypothotical business scenario (Coffee)
* Hyperledger fabric network for demo purposes including 1 org, 1 orderer, 1 peer
* SC project extraction to support plug and play on IBM cloud
* Mobile app prototype for consumers
### What left
* Hosting the SC project on a blockchain hosting provider
* API to query data from the mobile application
* Generate QR codes when the "Create" smart contract is sumbited
* Interate maps and history functionality to the mobile application 

## Name - Nipuna Weerasekara
### What Covered
* Initiated the CodeLabz project with ReactJS and Ant Design with the Firebase RTDB and Firestore as the backend.
* Implemented route protection for the React application.
* Implemented the cloud functions for email sending using Cloud Functions for Firebase and Firestore Email Trigger extension.
* Implemented social login functions with React-Redux-Firebase.
* Implemented push notification sending feature with Firebase Cloud Messaging.
* Created the GitHub action workflow for auto-deploy to Firebase hosting platform.
* Implemented the global state container using Redux, React-Redux, React-Redux-Firebase and Redux-Firestore.
* Added Firestore and Firebase database rules.
* Implemented the database periodic maintenance using Google Cloud Pub/Sub and Cloud Functions for Firebase.
* Implemented file upload to Cloud Storage for Firebase using React-Redux-Firebase.
* Implemented client-side full-text search using elasticlunr.
* Added Cypress test cases for UI automation testing.
### What left
* UI/UX improvements
* Add new push notification features

## Name - Omal Vindula
### What Covered
A mobile application built from ground-up using Flutter for the community with the following features.
* User registration and login for any user on the community app.
* Receiving and viewing dengue-prevention events published(past, present and future events) by the admins.
* Sending dengue incidents to the admins from the app.
* Viewing profile information and the sent incident reports to the admins.
* Integrating travis CI for the project
* Updating documentation

A web application developed from ground-up using React, Flask and MySQL as the Admin Panel for Dengue-Stop project with following features.
* User login only for the admins specified in the system.
* Viewing and verifying the incidents reported by the Community App to ensure their validity.
* Displaying metrics for dengue incidents and patients reported using a heat-map.
* Displaying graphs and visualizations of incidents reported over the time.
* Filtering, Sorting and Searching Dengue incidents/patients reported and look up their information.
* Changing status of dengue incidents reported based on the response of the admins.
* Creating dengue-prevention events for the public.
* Integrating travis CI for the project
* Updating documentation

A flask backend with MySQL database with folowing features.
* API endpoints to support functions required for both admin panel and community app.
* Interacting with MySQL database using flask-SQLAlchemy.
* Handling user authentication with JWT.
* Database migration and versioning using flask-migrate.
* Integrating travis CI for the project
* Updating documentation

### What left
* Deployment of Dengue Stop (Admin Panel, Flask Server, Community App)
* Adding multi-lingual support for Dengue Stop admin panel
* UI/UX improvements

## Name - Pasindu Kuruppuarachchi
### What Covered
D-IoT-A
* Design a DLT consortium cosnsit of 4 Organizations (For testign purposes) which includes the configuration of the Crypto-Assets and Configtx. [`PR-1`](https://github.com/scorelab/Bassa/pull/918)
* Introduced the HLF-Scaffold to the developement and deployment pipeline. [`PR-2`](https://github.com/leopardslab/d-iot-a/pull/2) 
* Chaincode for testing the implemented DLT network. [`PR-4`](https://github.com/leopardslab/d-iot-a/pull/4)
* Chaincode for Access Control Handling. [`PR-5`](https://github.com/leopardslab/d-iot-a/pull/5)

HLF-Scaffold
* Desiging of the system architecture [`Wiki`](https://github.com/leopardslab/hlf-scaffold/wiki/Architecture)
* Implemented HLF and prerequists installation shell scripts [`PR-1`](https://github.com/leopardslab/hlf-scaffold/pull/1/files)
* Implemented the Crypto Config Generator [`PR-3`](https://github.com/leopardslab/hlf-scaffold/pull/3/files) |
[`PR-4`](https://github.com/leopardslab/hlf-scaffold/pull/4/files)
* Implemented the Configtx generation using Python YAML library [`PR-5`](https://github.com/leopardslab/hlf-scaffold/pull/5/files)
* Set of YAML assets needed in network generation [`PR-6`](https://github.com/leopardslab/hlf-scaffold/pull/6/files)
* Introduced the Ruamel YAML library for YAML file handling. It preserseved the comments and order of YMAL structure in Fabric configurations. [`PR-7`](https://github.com/leopardslab/hlf-scaffold/pull/7)
### What left
* Docker-Compose generation
* Functions for editing a consortium definition. 
* Chaincode for adding Access Policies
* Packaging

## Name - Poornima Rangoda
### What Covered
* User login with Firebase authentication and authorization.
* Project creation for Crawling jobs.
* Crawling job scheduling.
* Backend integration with Django REST APIs.
* Message broker functionality for extensibility with RabbitMQ. 
* Job scheduling capability with Scrapy.
* Integrate data storing functionality with MongoDB.
* Platform wise centralized logs/query analysis with ElasticSearch. 
* Crawled data previewing. 
* UI for the CrawlerX platform with VueJS. 
### What left
* Upload crawling URLs from files.
* Kubernetes artifacts.

## Name - Ravindu De Silva
Chainkeepr analytic is a bitcoin mixing network detecting engine. Since it was the start of the project, the major requirements were to identify some trusted data sources, gather some required amount of data and conduct some graph-based data analysis on top of the data. The project had two phases. One is to gather the data and other one is to build the model. During the GSoC time period, I have discovered some trusted data sources, coded data crawlers, automated crawlers, modeled collected data into a graph, conducted an analysis on top of the modeled graph and built the primary analysis [model.](https://user-images.githubusercontent.com/20130001/90658529-4e34a700-e261-11ea-93bf-b53f0d906350.png)
### What done
Follow shows the summary of my contribution to the chain keeper analytic during GSoC 2020.
Data gathering crawlers
* Created bitcoinabuse and walletexplorer data gathering crawlers. [[PR-2]](https://github.com/scorelab/ChainKeeper-Analytics/pull/2)
* Optimized and debugged bitcoinabuse and walletexplorer and created the walletexplorer scan crawler. [[PR-3]](https://github.com/scorelab/ChainKeeper-Analytics/pull/3)
* Containerized BlockSci tool. [[PR-4]](https://github.com/scorelab/ChainKeeper-Analytics/pull/4)
 Data Analysis
* Analyzed the data (initial analysis of data).  [[PR-6]](https://github.com/scorelab/ChainKeeper-Analytics/pull/6)
* Community Detection Analysis [Domain-Bitcoin Address].  [[PR-7]](https://github.com/scorelab/ChainKeeper-Analytics/pull/7)
* Node classification with Node2Vec [bitcoin address vs domains vs pages] with TSNE clustering [bitcoin address vs domains vs pages].  [[PR-8]](https://github.com/scorelab/ChainKeeper-Analytics/pull/8) 
* Built graph prediction models (node2vec-link-prediction [bitcoin address vs domains vs pages]).  [[PR-9]](https://github.com/scorelab/ChainKeeper-Analytics/pull/9)
* Domain clustering with T-SNE dimension reduction and HC-agglomerative (single, complete, ward, average).  [[PR-11]](https://github.com/scorelab/ChainKeeper-Analytics/pull/11)
* Clustering graph nodes.  [[PR-12]](https://github.com/scorelab/ChainKeeper-Analytics/pull/12)

### What left
Following remaining works are not a part of my proposal but I see good potentials in them for a successor this project.
* Collect more trusted data sources and create data gathering crawlers to those sources. 
* Scale the graph (probably using a graph data based like arango DB or neo4j).
* Validate existing models.
* Build more models and validate them (Figure out retrain period, noise tolerance, accuracy, etc).

## Name - Rajitha Warusavitarana
###  What done
* Implemented parsers, transformers and generators in the code generation component for AWS, GCP and Azure. 
* Structuring the project as a monorepo with Yarn and Lerna.
* Created dummy data for unit testing and Wrote unit tests for the code generation component.
* Automating the API documentation process with JSDoc and Typescript compiler API.
* Updating the documentation of the NodeCloud project.
* Finalizing the `node-cloud.yml` file.
* Generating the JavaScript classes for NodeCloud plugins and updating the plugins with them.
### What left
* More cloud services can be generated by updating the `node-cloud.yml` file.

## Name - Sashika Nawarathne
### What Covered
- Created the OpenAPI specification
- Migrated the app to the new flask server
- Implemented image path tracking feature
- Updated multiple image uploading feature
- Integrated image editing feature
- Implemented project member management
- Implemented model training feature
- Updated image classification
- Created server handlers
- Implemented model versioning
- Add widget tests
- Updated the documentation
### What left
- Tests have to be completed

## Name - Shivanshu Raj Shrivastava
### What Covered
* Modify the current code base to make a strong robust command-line tool for OpenMF.
* Design logo and other frontend designs and components.
* Design and Implement a Client-side Framework for Web Client.
* Design and Implement Login, Admin, Management, and Extractor pages.
* Implementation of backend from scratch and writing different APIs in the flask framework.
* Extending the functionality of OpenMF to include management of files on the server.
* Design and implement a Database model, relation mapping (ORM) in the database to incorporate the above 
* functionalities in MySQL using the SQLAlchemy toolkit.
* Write a project wiki and update the user and developer documentation.
* Weekly blogs on medium.
### What left
* Some changes in the frontend to make it more user.
* Design and develop a logic to implement Analysis on the cases i.e. if in Case#1 and in Case#2 we have to search for common keyword "fire", then the Analytics API should check all the dbs and find the result. More complex scenarios can be introduced.
* More enhanced routing of the React App to provide better user experience

## Name - Tharaka Hewavitharana
### What Covered
- Adding Authentication and Authorization
- Adding Authorization clients like Google and Github
- Creating Spaces for gathering metrices for services
- Defining and developing Metrics gathering packages
- Implementing User interfaces for displaying metrics
- Defining time(Schedules) based checks for Mesuring up-time/down-time
- Implmenting package for corn jobs/ Scheduled checks
- Implementing map view for Region wife checks and application deployments
### What left
- Deploying the application in mutiple regions
- Conducting Regions wised checks

##  Name - Thisura Rathnayake
### What Covered
- Landing page (mobile + desktop)
- User registration, log in, password reset screens (mobile + desktop)
- Navbar (mobile + desktop)
- Footer (mobile + desktop)
- Page loading screen (mobile + desktop)
- Organization management screen (organization switcher sidebar, add users, edit organization details) (mobile + desktop)
- Crop images and upload component (mobile + desktop)
- View tutorial page (desktop only)
- Edit tutorial page (add/edit steps, add colors, real time collaboration, image scaling in the markdown) (desktop only)
### What left
- Tutorial details customization
- Organization public view
- Tutorial Feed
- HTML email

## Name - Vinuri Bandara
### What Covered
* Trending words and Word of the day.
* User registration and logins.
* Alphabetical indexing and search.
* Comment and report words.
* Adding new words and translations.
### What left
* Community dictionary users and moderator communication functionality. 
* User statistics and user involvement tracking.

