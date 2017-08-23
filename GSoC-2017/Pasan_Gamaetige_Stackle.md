# Stackle

## Student Info
* Name : Pasan Missaka
* Email : psn.missaka@gmail.com
* GitHub Profile : https://github.com/psnmissaka
* Country : Sri Lanka
* University : University of Colombo School of Computing


### Project Abstract
Stackle is an web communication portal aimed at providing Open Source organizations a platform to have discussions on their github projects and their issues. It provides Github intergration which allows adminstrator of an organization to create a forum thread for the particualr organization. Users signing in is able to view forums of the organizations they contribute to and engage in the forum discussions.

### [GSoC Project Page](http://LinikToYourGSoCProjectPage)

### [GSoC Project Proposal](https://goo.gl/QxGMjp)

### [GitHub Organization Repo](https://github.com/scorelab/Stackle)

### [GitHub Personal Repo](https://github.com/psnmissaka/Stackle)

### [Commits during GSoC 2017](https://github.com/scorelab/stackle/commits/master?author=psnmissaka)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/psnmissaka/Stackle/wiki)

### [GSoC Blog](http://GSoCBlog)

### Work Summary
Stackle was built from the ground up as a project for Google Summer of Code 2017. 

I started with developing the back-end API which is consumed by the Stackle front-end. NodeJS is used to handle the back-end logic 
with the use of Express framework. The API is mostly used to store data and retrieve data from the MongoDB server.
The front-end logic is developed using AngularJS. Front-end is designed to communicate with Stackle API and GitHub API to carry the business logic of the application.

### What Covered

* The authentication and authorization of users through Auth0 for GitHub users.
* Back-end API calls to get and store the data to the MongoDB (using mongoose)
* Front-end logic to subscribe to organizations, create posts regarding issues, search for organizations, creating a stack instance for a organization, display posts (by organization, by user), comment on posts and voting posts and comments.


### What left

* Notification handling mechanism
* Enable Gitlab login
* Sharing posts to social media

### Reference

1. [MongooseJS Documentation](http://mongoosejs.com/docs/guide.html)
2. [Routing with ExpressJS](http://expressjs.com/en/guide/routing.html)
3. [AngularJS](https://docs.angularjs.org/guide)
4. [GitHub API Documentation](https://developer.github.com/v3/)

