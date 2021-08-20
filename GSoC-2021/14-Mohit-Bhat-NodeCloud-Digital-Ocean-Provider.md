# NodeCloud- Digital Ocean Provider

# Student Info
- Name - Mohit Bhat
- Email - mbcse50@gmail.com
- University - Bennett University, Greater Noida
- GitHub Profile - https://github.com/mbcse
- LinkedIn profile - https://www.linkedin.com/in/mbcse/
- Medium - https://medium.com/@mbcse
- Twitter - mbcse50
- Project Link: [https://summerofcode.withgoogle.com/projects/#6697971531382784](https://summerofcode.withgoogle.com/projects/#6697971531382784)

# Project Abstract

<p align="center">
  <img src="https://raw.githubusercontent.com/leopardslab/nodecloud/master/assets/logo.png" >
</p>

NodeCloud is a standard library to get a single API on the open cloud with multiple providers. It is a NodeJs library which comes with plugins for each cloud provider. NodeCloud's aim is to abstract away the differences between different cloud providers. It provides an easy to use API for developers in order to interact with different cloud providers.

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6697971531382784)

## [GSoC Project Proposal](https://drive.google.com/drive/folders/1bzz5N9iHhIqGMtVCpADBy7G_XWeQk7np?usp=sharing)

## [GitHub Organization Repo](https://github.com/leopardslab/nodecloud)

## [GitHub Personal Repo](https://github.com/mbcse/nodecloud)

## [Commits during GSoC 2021](https://github.com/leopardslab/nodecloud/commits?author=mbcse)

## [Project Demo Video](https://youtu.be/Sd0L4qY-unQ)

## [Project Tracker During GSoC](https://www.notion.so/Google-Summer-Of-Code-2021-7e6cccd75dbe433b983202a1d09d0240)

## GSoC Blogs

- Community Bonding : [https://mbcse.medium.com/the-start-of-my-gsoc21-journey-cccb04b319e5](https://mbcse.medium.com/the-start-of-my-gsoc21-journey-cccb04b319e5)
- Week 1 Blog : [https://mbcse.medium.com/parsing-d-ts-files-using-typescript-compiler-week-1-gsoc21-8f9e794b9c63](https://mbcse.medium.com/parsing-d-ts-files-using-typescript-compiler-week-1-gsoc21-8f9e794b9c63)
- Week 2 Blog : [https://mbcse.medium.com/extracting-data-using-typescript-compiler-api-week-2-gsoc21-7c4adcf15fe2](https://mbcse.medium.com/extracting-data-using-typescript-compiler-api-week-2-gsoc21-7c4adcf15fe2)
- Week 3 Blog : [https://mbcse.medium.com/building-a-transformer-using-typescript-compiler-api-week-3-gsoc21-5db0bf95ad66](https://mbcse.medium.com/building-a-transformer-using-typescript-compiler-api-week-3-gsoc21-5db0bf95ad66)
- Week 4 & 5 Blog : [https://mbcse.medium.com/nodecloud-digital-ocean-services-and-testing-with-mocha-and-chai-week-4-5-gsoc21-ddec8a85f244](https://mbcse.medium.com/nodecloud-digital-ocean-services-and-testing-with-mocha-and-chai-week-4-5-gsoc21-ddec8a85f244)
- Week 6 Blog : [https://mbcse.medium.com/making-a-nodejs-module-and-workspace-management-with-lerna-week-6-gsoc21-79323e39e454](https://mbcse.medium.com/making-a-nodejs-module-and-workspace-management-with-lerna-week-6-gsoc21-79323e39e454)
- Week 7 & 8 Blog : [https://mbcse.medium.com/making-a-sdk-for-cloud-week-7-8-gsoc21-8e00b2e1c6b9](https://mbcse.medium.com/making-a-sdk-for-cloud-week-7-8-gsoc21-8e00b2e1c6b9)
- Week 9 & 10 Blog : [https://mbcse.medium.com/documenting-things-writing-example-and-the-git-week-9-and-10-the-ending-of-gsoc21-cf3b4127d042](https://mbcse.medium.com/documenting-things-writing-example-and-the-git-week-9-and-10-the-ending-of-gsoc21-cf3b4127d042)

# Work Summary

Nodecloud had support for AWS, Azure, and GCP. I worked on adding the support for Digital Ocean cloud. A plugin along with its code generation module is built. Digital Ocean has many third party SDK's out of which the best and suitable SDK Do-wrapper is used. I worked on making the parsers, generators and transformers using typescript compiler api to extract the classes and data(Like functions, parameters,comments, etc) from type definition files present in the digital ocean SDK. After auto generating the classes by the built tool, I made a digital ocean plugin out of it and added it to Nodecloud package. Now Nodecloud has support for Digital Ocean along with improved documentation.

# What Covered
- Added function for saving generated class files to their specific folders
- Created Parser for Digital ocean code generation module
- Created Generator for Digital ocean code generation module
- Created transformer for Digital ocean code generation module
- Wrote Unit Test for Parser, Transfomer and Generator
- Updated YML file for Digital Ocean Services
- Made Plugin for Digital Ocean 
- Implemented VPC and APPs service in Digital Ocean SDK
- Added scripts to run code generation tool easily
- Improved documentation explaining the Directory Structure, flow of tool and details of DO-plugin
- Wrote Examples for implemented Digital Ocean Services for Nodecloud

### Issues created

**[Update YML file to include digital ocean services](https://github.com/leopardslab/nodecloud/issues/95)** #95

**[Write examples for digital ocean plugin](https://github.com/leopardslab/nodecloud/issues/94)** #94 

**[Creating NodeCloud digital ocean plugin](https://github.com/leopardslab/nodecloud/issues/93)** #93 

**[Writing unit test for Digital Ocean generator](https://github.com/leopardslab/nodecloud/issues/92)** #92

**[Writing unit test for Digital Ocean transformer](https://github.com/leopardslab/nodecloud/issues/91)** #91

**[Writing unit tests for the Digital Ocean Parser](https://github.com/leopardslab/nodecloud/issues/90)** #90

**[Create generator for Digital Ocean code generation tool](https://github.com/leopardslab/nodecloud/issues/89)** #89 

**[Create Transformer for Digital Ocean Code Generation tool](https://github.com/leopardslab/nodecloud/issues/88)** #88 

**[Create parser for Digital Ocean code generation tool](https://github.com/leopardslab/nodecloud/issues/87)** #87


### Pull Requests

| Issue Name   |      Pull Request    |  Linked Issue |
|----------|:-------------:|------:|
| Digital Ocean Parser|  https://github.com/leopardslab/nodecloud/pull/96 | [#87](https://github.com/leopardslab/nodecloud/issues/87) |
| Digital Ocean transformer and generator |   https://github.com/leopardslab/nodecloud/pull/97  |   [#88](https://github.com/leopardslab/nodecloud/issues/88) [#89](https://github.com/leopardslab/nodecloud/issues/89) |
| Added unit tests for DO parser | https://github.com/leopardslab/nodecloud/pull/98 |    [#90](https://github.com/leopardslab/nodecloud/issues/90) |
| Added test for DO Transformer |    https://github.com/leopardslab/nodecloud/pull/99  |   [#91](https://github.com/leopardslab/nodecloud/issues/91) |
| Added tests for digital ocean Generator | https://github.com/leopardslab/nodecloud/pull/100 |    [#92](https://github.com/leopardslab/nodecloud/issues/92) |
| Added Digital Ocean Services to YML File |    https://github.com/leopardslab/nodecloud/pull/101  |   [#95](https://github.com/leopardslab/nodecloud/issues/95)  |
| Added Digital Ocean Plugin |    https://github.com/leopardslab/nodecloud/pull/102  |   [#93](https://github.com/leopardslab/nodecloud/issues/93)  |
| Added Examples for Digital Ocean NodeCloud-Plugin | https://github.com/leopardslab/nodecloud/pull/106 |    [#94](https://github.com/leopardslab/nodecloud/issues/94) |
| Updated Documentation for Nodecloud and Generator |    https://github.com/leopardslab/nodecloud/pull/107   |    |
| Final Changes and Issue's fixed(GSoC'21 Nodecloud Digital Ocean) | https://github.com/leopardslab/nodecloud/pull/108|   |


Do-wrapper SDK Pull Requests:
- https://github.com/matt-major/do-wrapper/pull/75
- https://github.com/matt-major/do-wrapper/pull/74


# What left
- Fixing problem with Database format in Do-wrapper SDK Implementation 
- Fixing issue with starting, stopping instance due to do-wrapper SDK implementation format
- Adding more services of digital ocean in YML file

# References
- [https://astexplorer.net/](https://astexplorer.net/)
- [https://ts-ast-viewer.com/](https://ts-ast-viewer.com/)
- [Writing typescript custom AST transformer part-1](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-1-7585d6916819)
- [Writing typescript custom AST transformer part-2](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-2-5322c2b1660e)
- [Writing typescript custom AST transformer part-3](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-3-93b6238ae21f)
- [https://developers.digitalocean.com/documentation/v2](https://developers.digitalocean.com/documentation/v2/#snapshots)