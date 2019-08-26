# nodecloud-web

## Student Info
  * Name - Amrita Chaturvedi
  * Email - amritachaturvedi97@gmail.com
  * GitHub profile - https://github.com/amrita019
  * LinkedIn profile - https://www.linkedin.com/in/amritachaturvedi/

### Project Abstract
NodeCloud is a standard library to get a single API on the open cloud with multiple providers. Making open cloud easily accessible and managed. The project aims to provides an interactive front end, where the user can access the capabilities of the SDK in a more convenient manner. It is containerized using docker. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/organizations/6311825751146496/?sp-page=3#5550327141498880)

### [GSoC Project Proposal](https://drive.google.com/file/d/1AKE_maXt8oUFeeu9kc5rsaMDL1u_NKeX/view?usp=sharing)

### [GitHub Organization Repo](https://github.com/cloudlibz/nodecloud-web)

### [GitHub Personal Repo](https://github.com/amrita019/nodecloud-web)

### [Commits during GSoC 2019](https://github.com/cloudlibz/nodecloud-web/commits/master?author=amrita019)

### [Project Demo Video](https://youtu.be/pvWIgoqe4YY)

### [Project Wiki](https://github.com/cloudlibz/nodecloud-web/wiki)

### [GSoC Blog](https://medium.com/my-gsoc-diary-with-score-lab)

### Work Summary
Developed a full-stack application for nodecloud. The server-end implemented in nodejs with express, was responsible for interacting with the database (using knexjs as SQL query builder), the nodecloud core sdk and it's plugins, namely nodecloud-azure-plugin, nodecloud-aws-plugin and nodecloud-gcp-plugin. The client-end implemented in react using redux, provided a user interactive dashboard.

### What Covered
* Create local database and server to which the front-end will corrospond to.
* Create UI Mockups
* Create authentication module, consisting of Login and Signup options. 
* User authentication done through jsonwebtoken (jwt)
* Create dashboard on frontend with functional Navbar, Sidebar and landing screen.
* List down the currently running azure services
* Add option to create Virtual Machine, Virtual Network, Database, Storage and Security
* Add an option to delete running services
* Write API documentation and project setup documentation
* Write unit tests for different functions

### What left
Component testing on client end

### After the GSoC
I would like to take care of nodecloud-web repository and would continue to commit.

### Reference
* [React JS](https://reactjs.org)
* [Redux](https://redux.js.org)
* [Node JS](https://nodejs.org/en/)
* [Express JS](https://expressjs.com)
* [Knex JS](http://knexjs.org/)
