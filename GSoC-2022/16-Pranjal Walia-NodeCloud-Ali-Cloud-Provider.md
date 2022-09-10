# NodeCloud- Digital Ocean Provider

# Student Info

- Name - Pranjal Walia
- Email - pranjalwalia77@gmail.com
- University - International Institute of Information Technology, Bangalore
- GitHub Profile - https://github.com/masterchief01
- LinkedIn profile - https://www.linkedin.com/in/pranjal-walia/
- Medium - https://medium.com/@pranjalwalia77
- Twitter - @PranjalWalia
- Project Link: [https://summerofcode.withgoogle.com/programs/2022/projects/l704UX9O](https://summerofcode.withgoogle.com/programs/2022/projects/l704UX9O)

# Project Abstract

<p align="center">
  <img src="https://raw.githubusercontent.com/leopardslab/nodecloud/master/assets/logo.png" >
</p>

NodeCloud is a standard library to get a single API on the open cloud with multiple providers. It is a NodeJs library which comes with plugins for each cloud provider. NodeCloud's aim is to abstract away the differences between different cloud providers. It provides an easy to use API for developers in order to interact with different cloud providers.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/l704UX9O)

## [GSoC Project Proposal](https://drive.google.com/file/d/1BYR_VZminLjZbCYpJsJskanSX4zSQQ0-/view?usp=sharing)

## [GitHub Organization Repo](https://github.com/leopardslab/nodecloud)

## [GitHub Personal Repo](https://github.com/masterchief01/nodecloud)

## [Commits during GSoC 2022](https://github.com/leopardslab/nodecloud/commits?author=masterchief01)

## [Project Demo Video](https://youtu.be/dD61Jb6IUqE)

## [Project Tracker During GSoC](https://complex-wall-1d1.notion.site/GSoC-22-SCoRe-Lab-34d63054e89f426fb380defddc630c32)

## GSoC Blogs

- Community Bonding : [https://medium.com/scorelab/google-summer-of-code-22-score-lab-community-bonding-period-2ed27d1b392a](https://medium.com/scorelab/google-summer-of-code-22-score-lab-community-bonding-period-2ed27d1b392a)
- Week 1 Blog : [https://medium.com/leopards-lab/coding-week-1-gsoc-22-with-score-lab-90937055e985](https://medium.com/leopards-lab/coding-week-1-gsoc-22-with-score-lab-90937055e985)
- Week 2 Blog : [https://medium.com/leopards-lab/coding-week-2-gsoc-22-with-score-lab-1f84c8995913](https://medium.com/leopards-lab/coding-week-2-gsoc-22-with-score-lab-1f84c8995913)
- Week 3 & 4 Blog : [https://medium.com/leopards-lab/coding-week-3-4-gsoc-22-with-score-lab-23f8dd0df940](https://medium.com/leopards-lab/coding-week-3-4-gsoc-22-with-score-lab-23f8dd0df940)
- Week 5 & 6 Blog : [https://medium.com/scorelab/coding-week-5-6-gsoc-22-with-score-lab-ebb88c3538a3](https://medium.com/scorelab/coding-week-5-6-gsoc-22-with-score-lab-ebb88c3538a3)
- Week 7 & 8 Blog : [https://medium.com/leopards-lab/coding-week-7-8-gsoc-22-with-score-lab-935dd83bd173](https://medium.com/leopards-lab/coding-week-7-8-gsoc-22-with-score-lab-935dd83bd173)
- Week 9 & 10 Blog : [https://medium.com/leopards-lab/coding-week-8-9-gsoc-22-with-score-lab-797576597add](https://medium.com/leopards-lab/coding-week-8-9-gsoc-22-with-score-lab-797576597add)

# Work Summary

The current implementation of NodeCloud is a core library that supports AWS, Azure, GCP and DigitalOcean cloud services as extensible plugins. I worked on extending this plugin functionality built into NodeCloud to include another emerging cloud provider i.e. Alibaba Cloud. The distribution of the project is in two major parts. First, implement the core functionalities of the AliCloud platform along with a suitable SDK that supports the latest OpenAPI specification. Second, the implementation of a code generation module to consume the SDK and auto-generate service implementations that can be assembled as the “alicloud-plugin” for NodeCloud integration. This is achieved by writing out parsers, generators and transformers specifically made for the SDK built out in the previous part. The built SDK is made public [here](https://github.com/masterchief01/alibabacloud-v2-typescript-sdk/) and is an unofficial alternative to the official SDK that still relies on the legacy API which is onward for deprecation.

# What Covered

- Added function for saving generated class files to their specific folders
- Created a Parser for the AliCloud code generation module
- Created a Generator for the AliCloud code generation module
- Created a transformer for the AliCloud code generation module
- Performed unit testing for the code generation module
- Updated the generator config file with sutaible AliCloud Services
- Finalized the plugin for the AliCloud Provider
- Implemented the Aliyun V2 TypeScript SDK for all core platform services
- Improved documentation explaining the Directory Structure, flow of tool and details of AliCloud
- Wrote Examples for implemented AliCloud Services for Nodecloud

### Issues created

**[Update existing documentation for Aliyun plugin usage](https://github.com/leopardslab/nodecloud/issues/142)** #142

**[Initialize the compute module](https://github.com/leopardslab/nodecloud/issues/133)** #133

**[Initialize Databases Module (sql+nosql)](https://github.com/leopardslab/nodecloud/issues/132)** #132

**[Initialize Networking Module](https://github.com/leopardslab/nodecloud/issues/131)** #131

**[Initialize Object Storage Module](https://github.com/leopardslab/nodecloud/issues/130)** #130

**[Add examples for Aliyun plugin usage](https://github.com/leopardslab/nodecloud/issues/128)** #128

**[Initialize NodeCloud Aliyun Plugin](https://github.com/leopardslab/nodecloud/issues/127)** #127

**[Tests for the Aliyun Generator](https://github.com/leopardslab/nodecloud/issues/126)** #126

**[Tests for the Aliyun Transformer](https://github.com/leopardslab/nodecloud/issues/125)** #125

**[Tests for the Aliyun Parser](https://github.com/leopardslab/nodecloud/issues/124)** #124

**[Create generator for Aliyun code generation tool](https://github.com/leopardslab/nodecloud/issues/123)** #123

**[Create Transformer for Aliyun code generation tool](https://github.com/leopardslab/nodecloud/issues/122)** #122

**[Create SDK parser for Aliyun code generation tool](https://github.com/leopardslab/nodecloud/issues/121)** #121

**[update generator config file](https://github.com/leopardslab/nodecloud/issues/120)** #120

### Pull Requests

| **Issue Name**                                    | **Pull Request**                                  | **Linked Issue**                                                                                                                                                                                                                                |
| ------------------------------------------------- | ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| update formatter conf and apply formatter         | https://github.com/leopardslab/nodecloud/pull/137 | [#116](https://github.com/leopardslab/nodecloud/issues/116)                                                                                                                                                                                     |
| Aliyun parser                                     | https://github.com/leopardslab/nodecloud/pull/138 | [#121](https://github.com/leopardslab/nodecloud/issues/121) [#124](https://github.com/leopardslab/nodecloud/issues/124)                                                                                                                         |
| Addition of transformations to generator          | https://github.com/leopardslab/nodecloud/pull/139 | [#122](https://github.com/leopardslab/nodecloud/issues/122) [#123](https://github.com/leopardslab/nodecloud/issues/123) [#125](https://github.com/leopardslab/nodecloud/issues/125) [#126](https://github.com/leopardslab/nodecloud/issues/126) |
| AliCloud Provider: Storage                        | https://github.com/leopardslab/nodecloud/pull/140 | [#127](https://github.com/leopardslab/nodecloud/issues/127)                                                                                                                                                                                     |
| Package Aliyun Services                           | https://github.com/leopardslab/nodecloud/pull/141 | [#127](https://github.com/leopardslab/nodecloud/issues/127) [#120](https://github.com/leopardslab/nodecloud/issues/120)                                                                                                                         |
| Added Examples for AliCloud NodeCloud-Plugin      | https://github.com/leopardslab/nodecloud/pull/144 | [#128](https://github.com/leopardslab/nodecloud/issues/128)                                                                                                                                                                                     |
| Updated Documentation for Nodecloud and Generator | https://github.com/leopardslab/nodecloud/pull/143 | [#142](https://github.com/leopardslab/nodecloud/issues/142)                                                                                                                                                                                     |

Aliyun V2 SDK:

- https://github.com/masterchief01/alibabacloud-v2-typescript-sdk
- https://www.npmjs.com/package/aliyun-v2-typescript-sdk

# What left

- Pending OpenAPI spec update by AliCloud for Aliyun Kubernetes (ACK)
- Adding more services of AliCloud in generator config file

# References

- [https://astexplorer.net/](https://astexplorer.net/)
- [https://next.api.alibabacloud.com/api](https://next.api.alibabacloud.com/api)
- [https://ts-ast-viewer.com/](https://ts-ast-viewer.com/)
- [Writing typescript custom AST transformer part-1](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-1-7585d6916819)
- [Writing typescript custom AST transformer part-2](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-2-5322c2b1660e)
- [Writing typescript custom AST transformer part-3](https://levelup.gitconnected.com/writing-typescript-custom-ast-transformer-part-3-93b6238ae21f)
