# GoCloud
## Student Info
* Name - Pratik Dhanave
* Email - i.pratikdhanave@gmail.com
* GitHub profile - https://github.com/PratikDhanave

### Project Abstract
gocloud is a standard library for Go that abstracts away differences among multiple cloud providers. The gocloud compute package is designed to make it easy to provision and work with VMs. Developing golang package for interacting with Google compute engine and AWS EC2 using a unified API.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5679856277782528)

### [GSoC Project Proposal](https://docs.google.com/document/d/1ZmVHT4vgxPcft7XZj8dInYof51uu32hWEkszuAZUy3E/edit)

### [GitHub Organization Repo](https://github.com/scorelab/gocloud-v2/)

### [GitHub Personal Repo](https://github.com/PratikDhanave/gocloud-v2)

### [Commits during GSoC 2017](https://github.com/scorelab/gocloud-v2/commits/master?author=PratikDhanave)

### [Project Demo Video](https://www.youtube.com/playlist?list=PLOdfztY25UNnxK_0KRRHSngJIyVLDKZxq)

### [Project Wiki](https://github.com/PratikDhanave/gocloud-v2/wiki)

### [GSoC Blog](https://pratikdhanave.github.io/blog/2017/08/27/gocloud-google-summer-of-code-final-report/)

### Work Summary
For GSoC 2017 I have initiated the project from scratch and added support for AWS and Google cloud platform (GCP).

Support for following services were added,
- Compute
- Storage
- Container
- Load Balancing
- DNS
- for authentication with AWS cloud I implemented signature-version-2 and signature-version-4 method.
- for authentication with Google cloud I implemented OAuth client and  service account authentication method.

Along with development of APIs, I added documentation and unit tests.
Created tutorial series.

### What Covered

- Developed APIs for compute, Storage, Container, Load Balancing and DNS services.

	1. AWS
		- EC2
		- AWS Storage Service
		- Amazon Elastic Container Service(ECS) 
		- AWS Elastic Load Balancing
		- AWS Route5S
	2. GCP
		- Compute(GCE)
		- Google Storage Service
		- Google Container Service (Container)
		- Google Elastic Load Balancing
		- Google Cloud DNS

- Added unit tests for developed APIs.
- Added documentation for developed APIs.
- Added examples for developed APIs.
- Added Developer API documentation using godoc for developed APIs.
- Created gocloud getting started video tutorial series.

### What left

- Additional APIs can be added as improvements in next versions.
- Potential to add more cloud providers.

### Reference

- [Aws-documentation](https://aws.amazon.com/documentation/)
- [Aws-signature-version-2](http://docs.aws.amazon.com/general/latest/gr/signature-version-2.html)
- [Aws-signature-version-4](http://docs.aws.amazon.com/general/latest/gr/signature-version-4.html)
- [Google-cloud-documentation](https://cloud.google.com/docs/)
- [AWS and Google Cloud platform comparison](https://cloud.google.com/docs/compare/aws/)



