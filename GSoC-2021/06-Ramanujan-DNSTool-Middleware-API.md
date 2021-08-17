# DNSTool Middleware/API

## Student Info

- Name - Ramanujan
- Email - [w.nipuna@gmail.com](mailto:w.nipuna@gmail.com)
- GitHub Profile - [Niweera](https://github.com/Niweera)
- Medium - [@niweera](https://medium.com/@niweera)
- Twitter - [@Niweera](https://twitter.com/Niweera)

## Project Abstract

_DNSTool_ is a system to monitor a given set of internet resources such as Domains, IPs, etc. The **DNSTool
Middleware/API** is the main component that manages the core processing and obtaining of scan lists and their respective
scan results. **DNSTool Middleware/API** acts as a bridge between the user interface and the back-end system.

![image](https://user-images.githubusercontent.com/20130001/119268942-cbd37c00-bc12-11eb-8f65-55e5abb7d66a.jpg)

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5396149764096000)

## [GSoC Project Proposal](https://drive.google.com/file/d/16F45RKFMZHErYxk5Aza8awihx6ARROlL/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/DNSTool-Middleware-API)

## [GitHub Personal Repo](https://github.com/Niweera/DNSTool-Middleware-API)

## [Commits during GSoC 2021](https://github.com/scorelab/DNSTool-Middleware-API/commits?author=Niweera)

## [Project Demo Video](https://www.youtube.com/watch?v=EEjBEaHIrbA)

## [Project Wiki](https://github.com/scorelab/DNSTool-Middleware-API/blob/main/api-gateway/WIKI.md)

## GSoC Blog

- [GSoC 2021 with SCoRe Lab](https://medium.com/scorelab/gsoc-2021-with-score-lab-119d5b6e37b9)
- [GSoC 2021 with SCoRe Lab — Week 1](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-1-6217437d4b55)
- [GSoC 2021 with SCoRe Lab — Week 2](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-2-4f9c640e9a2b)
- [GSoC 2021 with SCoRe Lab — Week 3](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-3-69c3cf32ec0c)
- [GSoC 2021 with SCoRe Lab — Week 4](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-4-9b0913cdd21d)
- [GSoC 2021 with SCoRe Lab — Week 5](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-5-e65740c1b42)
- [GSoC 2021 with SCoRe Lab — Week 6](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-6-410e34dbcb5c)
- [GSoC 2021 with SCoRe Lab — Week 7](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-7-fad037bec8de)
- [GSoC 2021 with SCoRe Lab — Week 8](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-8-48a4a21c71af)
- [GSoC 2021 with SCoRe Lab — Week 9](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-9-3f4c7a7474f8)
- [GSoC 2021 with SCoRe Lab — Week 10](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-10-56b0d48abf47)
- [GSoC 2021 with SCoRe Lab — Week 11](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-11-fb70657f45a6)
- [GSoC 2021 with SCoRe Lab — Week 12](https://medium.com/scorelab/gsoc-2021-with-score-lab-week-12-713f0ded9315)

## Work Summary

Over the course of GSoC 2021, I implemented the DNSTool-Middleware-API Gateway. The DNSTool-Middleware-API Gateway is
developed using Python language using the Flask web framework. The database used for the API Gateway is Google Firebase
Realtime Database. I created the database schema for the API Gateway using Firebase Realtime Database. I used
Flask-RESTful library to implement the API Gateway as a RESTful API. I used Flask Caching to add the Caching feature to
the Flask application. I implemented the user registration feature using Google Firebase Authentication and I
implemented the email sending functionality where when the user registration is successful, the user will be greeted
with a welcome email. In addition, I implemented the feature to download scan results files using Google Cloud Storage
Python library and Flask Streaming API. I used OpenAPI v3.0 Swagger UI to document the API endpoints in
DNSTool-Middleware-API Gateway. I used Flask testing library to test the functionality of the Flask application.

## What Covered

1. Initiated DNSTool-Middleware-API Gateway using Python Flask and using Google Firebase Realtime Database.
2. Implemented authentication middleware for the Flask API endpoints.
3. Added JWT authentication and validation for Firebase Authentication.
4. Added Google reCAPTCHA v3 protection for the API endpoints where human interaction is vital (example: user
   registration).
5. Implemented email sending functionality using Flask-Email library.
6. Added Firebase Realtime Database rules to protect the database from unauthorized access.
7. Documented all the endpoints and their functionalities using OpenAPI v3.
8. Implemented file stream downloading using Google Cloud Storage and Flask Streaming API.
9. Implemented user authentication workflow DNSTool-CLI (See below for authentication workflow).
10. Implemented service account generation for user authentication using PyCryptodome and PyJWT libraries.
11. Created deploy scripts for the DNSTool-Middleware-API Gateway using Terraform and Ansible and deployed in an Ubuntu Virtual Machine hosted in Google Cloud Platform using NGINX as the reverse proxy.
12. Added test cases for the Flask application using Flask testing library.

![image](https://camo.githubusercontent.com/9cce3ca92c78436afce5a043504ea5ac7d28ed30dd5dd26169c5127575345b31/68747470733a2f2f692e696d6775722e636f6d2f50434755444a4c2e706e67)

## What left

1. Add SSL certificate to the DNSTool-Middleware-API Gateway

## References

1. [Flask](https://flask.palletsprojects.com/en/2.0.x/)
2. [Flask-RESTful](https://flask-restful.readthedocs.io/en/latest/)
3. [OpenAPI v3 - Swagger](https://swagger.io/specification/)
4. [Firebase Realtime Database](https://firebase.google.com/docs/database)
5. [Firebase Authentication](https://firebase.google.com/docs/auth)
6. [Google Cloud Storage](https://cloud.google.com/storage)
7. [Google reCAPTCHA v3](https://developers.google.com/recaptcha/docs/v3)
8. [Terraform](https://www.terraform.io/)
9. [Ansible](https://www.ansible.com/)
10. [PyCryptodome](https://pycryptodome.readthedocs.io/en/latest/)
11. [PyJWT](https://pyjwt.readthedocs.io/en/stable/)
12. [JWT](https://jwt.io/)
13. [Google Cloud Platform](https://cloud.google.com/)
14. [NGINX](https://www.nginx.com/)
15. [DNSTool-Middleware-API Live Demo](https://api.procyberintel.com/docs/)