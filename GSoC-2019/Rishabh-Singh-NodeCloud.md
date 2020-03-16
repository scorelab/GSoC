# Nodecloud - DigitalOcean & AliCloud

## Student Info
  * Name - Rishabh Singh
  * Email - pingrishabh@gmail.com
  * GitHub profile - https://github.com/cheesetouched
  * LinkedIn profile - https://www.linkedin.com/in/pingrishabh
  
### Project Abstract
NodeCloud is Node.js based API for open cloud. It works as a standalone core and depends on the cohesive plugins that extends its support onto different cloud providers. Currently, NodeCloud supports AWS, Google Cloud Platform and Azure and houses a handy plugin for all the three providers.

With GSoC ‘19, I aimed to extend the provider paradigm of NodeCloud, by expanding to DigitalOcean & AliCloud.

Each provider supplies NodeCloud with variety of implementable products. Some of these products that are available in NodeCloud are:
  * Compute
  * Storage
  * Networking
  * Databases
  * Security/ Authorization
  * Utilities


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4928846581727232)

### [GSoC Project Proposal](https://docs.google.com/document/d/1ApSt8RShhIczdwSi-a-IYj7N4HKnRDWpSe20vFWYCTw/edit?usp=sharing)

### GitHub Organization Repo
  * [nodecloud-ali-plugin](https://github.com/cloudlibz/nodecloud-ali-plugin)
  * [nodecloud-digitalocean-plugin](https://github.com/cloudlibz/nodecloud-digitalocean-plugin)

### GitHub Personal Repo
  * [nodecloud-ali-plugin](https://github.com/Cheesetouched/nodecloud-ali-plugin)
  * [nodecloud-digitalocean-plugin](https://github.com/Cheesetouched/nodecloud-digitalocean-plugin)

### Commits during GSoC 2018
  * [nodecloud-ali-plugin](https://github.com/cloudlibz/nodecloud-ali-plugin/commits?author=Cheesetouched)
  * [nodecloud-digitalocean-plugin](https://github.com/cloudlibz/nodecloud-digitalocean-plugin/commits?author=Cheesetouched)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/cloudlibz/nodecloud/projects/3)

### [GSoC Blog](https://medium.com/nodecloud-19)

### Work Summary
Two cloud services - DigitalOcean & AliCloud, were successfully added to Nodecloud as providers and are added to the list of plugins. The individual repositories for these plugins exist in GitHub and can be easily accessed and modified according to the requirements. New integrations can be easily supported by these plugins due to the laid boilerplate during development. Users can simply import these plugins using nodecloud-core and get started. Use-case based examples are shipped with each plugin for each module and for each action. These can be simply copied and pasted by beginners to achieve various end results. 

### What Covered
  * AliCloud - Read Me
  * AliCloud - Controller
  * AliCloud - Compute Module
  * AliCloud - Database Module
  * AliCloud - Networking Module
  * AliCloud - Storage Module
  * AliCloud - Examples Folder
  * AliCloud - Unit Tests
  * AliCloud - Mock Level SDK
  * DigitalOcean - Read Me
  * DigitalOcean - Controller
  * DigitalOcean - Account Module
  * DigitalOcean - Compute Module
  * DigitalOcean - Networking Module
  * DigitalOcean - Storage Module
  * DigitalOcean - Examples Folder
  * DigitalOcean - Integration Tests
  * DigitalOcean - Unit Tests
  * DigitalOcean - Mock Level SDK

### What left
  * <del> A little bit of unit testing for AliCloud
  * <del> Pushing a stable AliCloud source to GitHub
  * <del> User-friendly documentation for the beginners

### After GSoC
There are several exciting features and integration-worthy modules that I came across while scraping the respective SDKs. These features are of absolute importance in isolation and would be a great addition to the respective plugins. Although, due to strict and confined schedule, I could not have integrated them while staying on track with the schedule at the same time. So I would love to stay in touch with Nodecloud and become an active contributor after GSoC ends. I aim to slowly and steadily add these modules to the respective plugins one-by-one. I also wish to become the maintainer of these plugins and publish them to npm.

### Reference
* [Nodecloud Core](https://github.com/cloudlibz/nodecloud)
* [Nodecloud AWS Plugin](https://github.com/cloudlibz/nodecloud-aws-plugin)
* [DigitalOcean SDK](https://www.npmjs.com/package/digitalocean)
* [AliCloud SDK](https://www.npmjs.com/package/@alicloud/pop-core)
* [Node JS](https://nodejs.org/en)
* [Jest](https://jestjs.io)
