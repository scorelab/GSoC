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
### Milestone 1-

<br/>
<div align="center">
<br/>

![OAuth2 authentication using google and github](https://user-images.githubusercontent.com/43586052/87230775-a3aea600-c3cf-11ea-8b33-5dd4e0211395.gif)
<br/>

![ER-Design](https://user-images.githubusercontent.com/43586052/84043084-8008d200-a9c3-11ea-9ba4-886ad51e489f.png)
</div>
<br/>

- [x] Finalize the idea and structure of the project.
- [x] Set up basic layout of the backend server Flask and integrate the database.
- [x] Start writing new models.
- [x] Write Auth, Projects, Labels, Images, Users routes.
- [x] Add authentication using access and refresh tokens.
- [x] Implement user token as well as OAuth2 based authentication with Google,  Facebook, GitHub.
- [x] Start writing tests for existing frontend in react and redux and for the backend.
- [x] Complete documentation for the labeller.

### Milestone 2-

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
### Reference
- [Google Maps Api Platform](https://developers.google.com/maps/documentation)
- [Docker documentation](https://docs.docker.com/)