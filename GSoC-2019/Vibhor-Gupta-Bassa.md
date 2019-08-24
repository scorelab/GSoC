# Bassa: File Management and ACL

## Student Info  

  * Name - Vibhor Gupta
  * Email - vibhordelgupta@gmail.com
  * University - Delhi Technological University
  * GitHub profile - https://github.com/VibhorCodecianGupta
  * LinkedIn profile - https://www.linkedin.com/in/vibhor-gupta-357458134/  


### Project Abstract  
To scale Bassa from its current use of an internet download queueing micro-service to a full-fledged file management system for uploading resources on the local server in an organised fashion of folders and directories for better maintainability. To design and develop a flow of sharing resources via custom link generation and granting varied access to users and user groups (another planned feature) based on an ACL model. The vision of the proposal is to take a leap toward a cloud-based storage service for resources, similar to existing drive services.  


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4645813739847680)

### [GSoC Project Proposal](https://drive.google.com/file/d/1m3HAPvk0J_rC8NF-DVDMxxLedYYz3Yrf/view)

### [GitHub Organisation Repo](https://github.com/scorelab/Bassa)

### [GitHub Personal Repo](https://github.com/VibhorCodecianGupta/Bassa)

### [Commits during GSoC 2019](https://github.com/scorelab/Bassa/pull/818/commits)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/scorelab/Bassa/wiki/File-Management-System)

### Work Summary  
  Designed and developed a full stack file management flow for users, with CRUD functionality on resources according to an ACL based permission model wherein users can share resources with other users with restricted access. The owned and shared resources are separately displayed with seamless navigation and permission granting flow. The users can also upload files to server, add folders and move resources around. The users would receive broadcasted notifications when their queued downloads are complete, their signup requests are approved and when they are granted access to some resource.

### What's Covered
  1. Added models for resource entity and ACL structs.  
  2. Designed database relations and wrote SQL script for the same.
  3. Added APIs for CRUD operations on resource entities.
  4. Added endpoints for permission checks and grants.
  5. Revamped the entire database and API flow according to composite design pattern.
  6. Added file upload support and notification broadcasting APIs.
  7. Designed a global parent and permission context stack service on the frontend to manage resource navigation.
  8. Wrote services and controllers for CRUD operations on resources with permission checks and maintaining stack context on every user action (to ensure proper flow of permissions in the directory tree).
  9. Wrote Notification services and pollers to fetch and save notifications.
  10. Implemented Upload support on the frontend to relay multipart form-data to backend and upload it to server.
  11. Wrote the boilerplate frontend for the aforementioned functions.

### What's left/ After GSoC
  1. Checks on file uploads such as limits and ZIP compressions.
  2. Uploading folders.
  3. User group construct to better manage permission grants.

### Reference
  1. [Composite Design pattern](https://refactoring.guru/design-patterns/composite)
  2. [AngularJS documentation](https://code.angularjs.org/1.1.2/docs/api)
  3. [Project Structure and flow](https://scotch.io/tutorials/angularjs-1-x-fundamentals-part-1#toc-supports-dependency-injection)
  4. [Material library for AngularJS](https://material.angularjs.org/latest/getting-started)
