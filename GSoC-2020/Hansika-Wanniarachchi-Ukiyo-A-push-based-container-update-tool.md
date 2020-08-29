# Ukiyo - A push based container update tool

## Student Info

* Name - Hansika Wanniarachchi
* Email - hansijw76@gmail.com
* University - University of Moratuwa, Sri Lanka
* GitHub Profile - https://github.com/HansikaW 
* Medium - https://medium.com/@HansikaWanniarachchi

### Project Abstract

ukiyo is a push based container update tool that acts as a watcher for docker containers. It will run alongside with the other running containers and will be responsible for automatic updates and schedule container deployment time. Push events will be received from ukiyo via the docker registry webhook to updated the containers. ukiyo itself runs as a Docker container or else runs as a separate background process a daemon.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5966531676078080)

### [GSoC Project Proposal](https://docs.google.com/document/d/1Oc37N0PLzrosCgDIjE3lNB3E0eYa22ZIIHJ8QsYsbS8/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/leopardslab/ukiyo)

### [GitHub Personal Repo](https://github.com/HansikaW/ukiyo)

### [Commits during GSoC 2020](https://github.com/leopardslab/ukiyo/commits?author=HansikaW)

### [Project Demo Video](https://drive.google.com/file/d/1AsjIcbLw9I8kf_h2IHG2exAr12GpW5Gs/view?usp=drivesdk)

### [GSoC Blog](https://medium.com/@HansikaWanniarachchi/gsoc-2020-work-summary-70c9db9a5e1c)

### [Project Wiki](https://github.com/HansikaW/ukiyo/wiki)

### Work Summary

This project was conducted in order to implement a lightweight agent run on the docker which facilitate push-based solution for automating container deployment. Push events will be received from ukiyo via webhooks. Docker registries provide webhooks to subscribe and listen to image changes. Locally running images will change only after such an event is received by ukiyo. Ukiyo support for the multiple Docker Registries and It will pull the latest images and make the deployment according to the instruction. ukiyo will automatically complete the deployment on the fly or at the scheduled time and all deployment events loaded into own cache. Ukiyo support to expose multiple external ports and maintain a log file thus users can view the cache data using CLI command. Not only that, but the user can view the status of the scheduled events in a table view. ukiyo container run alongside with the other running containers.

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

### Reference

- [Docker Documentation](https://docs.docker.com/)
- [Docker Swam](https://docs.docker.com/engine/swarm/)
- [Go DockerClient](https://github.com/fsouza/go-dockerclient)
