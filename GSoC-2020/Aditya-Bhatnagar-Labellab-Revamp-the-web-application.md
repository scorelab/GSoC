# Labellab - Revamp the web application

## Student Info

* Name - Aditya Bhatnagar
* Email - abhatnagar@mt.iitr.ac.in
* University: Indian Institute of Technology Roorkee, India
* GitHub Profile - https://github.com/carpecodeum
* Medium - https://medium.com/@abhatnagar_91984
* LinkedIn Profile: https://www.linkedin.com/in/aditya-bhatnagar-2421a3178/

### Project Abstract
LabelLab is an image labeling tool for a researcher. It was started with a vision to classify and label all kinds of images of animals. But now it has expanded enough to incorporate other types of images as well. It can handle labeling bulks of images of different formats in order to be used for supervised learning. It will also have the features to run classifications to train a model and display the necessary information. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6532632877203456)

### [GSoC Project Proposal](https://docs.google.com/document/d/1FIRq3i_d8f51hrP0tymkAGzyA8v7C0C-A6HSndvnm5Y/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/LabelLab)

### [GitHub Personal Repo](https://github.com/carpecodeum/LabelLab)

### [Commits during GSoC 2020](https://github.com/scorelab/LabelLab/commits?author=carpecodeum)

### [GSoC Blog](https://medium.com/@abhatnagar_91984)

### Work Summary
This is a comprehensive list of the milestones that were achieved for Revamping the Backend-
### Milestone 1- (Issue #283)
- [x] Finalize the idea and structure of the project.
- [x] Set up basic layout of the backend server Flask and integrate the database.
- [x] Start writing new models.
- [x] Write Auth, Projects, Labels, Images, Users routes.
- [x] Implement user token as well as OAuth2 based authentication with Google,  Facebook, GitHub.
- [x] Start writing tests for existing frontend in react and redux and for the backend.
- [x] Complete documentation for the labeller.
### Milestone 2- (Issue #283)
- [x] Implement the functions to convert data to be displayed as statistical diagrams.
- [x] Write Analytics and Classification routes.
- [x] Complete making the Image formatting/editing tool.
- [x] Implement the Team feature inside the projects. Including the changes needed to the frontend.
- [x] Complete the tests for the code base.
### Milestone 3-
- [x] Implement Path-racking feature.
- [x] Marking of latitudes and longitudes extracted from the image's metadata with Polylines feature of Google maps and custiomize it to meet the needs of the project.
- [x] Dockerize the LabelLab Flask server edit the existing docker-compose file for the frontend changes.
- [x] Prepare to Deploy the containerized app to GCP
- [x] Integrating the two builds and test cases with Travis.
- [x] Fix bugs and polish the new features and review the documentation.

### What Covered

### What left
- Full deployment of the already dockerized and deployement ready app.
- Completion of some parts of the Sphinx documentation.
### Reference
- [Google Maps Api Platform](https://developers.google.com/maps/documentation)
- [Docker documentation](https://docs.docker.com/)