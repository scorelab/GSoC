# Project Name

## Student Info

- Name - OddCN ( Junqiu Zheng )
- Email - oddcn.zheng@gmail.com
- GitHub profile - https://github.com/OddCN

### Project Abstract

GoCloud is a standard library for Go that abstracts away differences among multiple cloud providers. Developing golang package for interacting with Google cloud, AWS, Digital Ocean, Ali-cloud, Vultr using a unified API.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6225862895075328)

### [GSoC Project Proposal](https://docs.google.com/document/d/1lCiUWSqlW1ubbF6exvuIGePvYE949f0Ep1AhP234aT4/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/cloudlibz/gocloud)

### [GitHub Personal Repo](https://github.com/OddCN/gocloud)

### [Commits during GSoC 2018](https://github.com/cloudlibz/gocloud/commits?author=OddCN)

### Project Demo Video

[Ali-cloud tutorial videos](https://www.youtube.com/playlist?list=PLcDQypWNHCeiym0jmezozjQhEbe84oh-q)

[Vultr tutorial videos](https://www.youtube.com/playlist?list=PLcDQypWNHCeiXMQZBmfIKTeYTWYUdWVwj)

### [Project Wiki](https://github.com/cloudlibz/gocloud/wiki)

### [GSoC Blog](https://medium.com/gocloud)

### Work Summary

In GSoC 2018, I implemented Ali-cloud and Vultr support for GoCloud. And other works: GoCloud modular, builder pattern for inputting, parsing response.

Support for following services of Ali-cloud were implemented:

- ECS Compute
- ECS Storage
- Alibaba Cloud DNS
- Server Load Balancer
- Container Service

Support for following services of Vultr were implemented:

- Server
- Bare Metal
- Block Storage
- DNS

For every implementation of services/modules and functions, contains unit tests, API documentations, example documentations and getting start tutorial videos.

### What Covered

#### Ali-cloud and Vultr support

For Ali-cloud, developed APIs of compute, storage, container service, load balancer, DNS services.

For Vultr,  developed APIs of compute, storage, bare metal, DNS services.

Added unit tests, API documentations, example documentations and getting start tutorial videos for implemented services of Ali-cloud and Vultr.

#### GoCloud modular

Achieved three goals:

- way to call: `GoCloud.<ServiceType>.<Functionality>`
- development scalable
- ensure the API is uniform like before

[More information](https://medium.com/gocloud/gocloud-modular-scalable-db61160138aa)

#### Builder pattern for inputting parameters

Achieved four goals:

- Prevent user from inputting wrong parameter name
- Throw an error when user miss input required parameters
- Let user add parameters in different places
- Let user have higher freedom, clearer code

[More information](https://medium.com/gocloud/gocloud-using-builder-pattern-to-improve-user-experience-f5cc2f79c9f4)

#### Parsing response

Achieved two goals:

- users get the response struct directly
- put HTTP/HTTPS status code into response struct

[More information](https://medium.com/gocloud/gocloud-work-summary-d809d11c8a14)

### What left

- Additional APIs can be added as improvements
- Builder pattern for more cloud providers
- Parsing response for more cloud providers

### Reference

[Alibaba Cloud Document Center](https://www.alibabacloud.com/help/)

[Vultr API Reference](https://www.vultr.com/api/)