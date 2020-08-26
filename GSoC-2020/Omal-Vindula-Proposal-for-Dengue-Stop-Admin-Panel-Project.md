# Dengue Stop Community Application and Admin Panel

## Student Info

* Name - Omal Vindula
* Email - omalvindula@live.com
* GitHub Profile - https://github.com/DonOmalVindula
* Medium - https://medium.com/@omalwijegunawardana
* Twitter - https://twitter.com/omal_vindula

### Project Abstract

Dengue Stop is a project which helps medical officials to monitor the dengue incidents and metrics all over the world/country using Dengue Stop Admin Panel, in a meaningful manner so that they could make informed decisions based on good quality data that is being provided by the Dengue Stop community application.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6293985435320320)

### [GSoC Project Proposal](https://docs.google.com/document/d/1Cp9IHIpCbrQw_61pJ5UA00F-8laT-C9fY3tlhjx6gp4/edit?usp=sharing)

### [GSoC Project Proposal Revisions](https://docs.google.com/document/d/1Yhu3SrcbS6-3lBwCDFJQ2sGnQfRRdk_eN8BZ1VZ5vXM/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/DengueStop)

### [GitHub Personal Repo](https://github.com/DonOmalVindula/DengueStop)

### [Commits during GSoC 2020](https://github.com/scorelab/DengueStop/commits?author=donomalvindula)

### [Project Demo Video](https://youtu.be/eGlVXmKyJw8)

### [GSoC Blog](https://medium.com/@omalwijegunawardana/consolidated-gsoc-blogs-e9adc59b4628)

### Work Summary
During GSoC 2020, I have covered almost all the planned milestones. The project had 3 main deliverables as listed below.

* A Flutter community app to report dengue incidents happening around them and to get notified of initiatives done by officials for dengue prevention.
* An Admin Panel using React.js to view and analyze dengue incidents and patients reported by the community.
* A Flask backend with MySQL database to support both dengue stop community app and the admin panel.

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

### Reference
* [Flutter Documentation](https://flutter.dev/docs)
* [Reactjs Documentation](https://reactjs.org/docs/getting-started.html)
* [Flask Documentation](https://flask.palletsprojects.com/en/1.1.x/)
* [Flask-SQLAlchemy Documentation](https://flask-sqlalchemy.palletsprojects.com/en/2.x/)
* [Python Documentation](https://docs.python.org/3/)
