# NodeCloud

## Student Info

* Name - Tharaka Romesh Hewavitharana
* Email - tharakaromesh@gmail.com
* GitHub profile - https://github.com/TRomesh
* Twitter - [@DTRomesh](https://twitter.com/DTRomesh)

### Project Abstract

NodeCloud is a standard library to get a single API on the open cloud with multiple providers. Making open cloud easily accessible and managed. The proposed system would be improving the existing feature as well as adding new features and cloud providers.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5556288790986752)

### [GSoC Project Proposal](https://docs.google.com/document/d/1ForylQD_kBKUZQbO458xy91bT_LxoE1Z9GmCuz1SufY)

### [GitHub Organization Repo](https://github.com/cloudlibz/nodecloud-cli)

### [GitHub Personal Repo](https://github.com/TRomesh/nodecloud-cli)

### [Commits during GSoC 2019](https://github.com/cloudlibz/nodecloud-cli/commits/master?author=TRomesh)

### [Project Demo Video](https://www.youtube.com/watch?v=A8UAJluShPE)

### [GSoC Blog](https://medium.com/nodecloud)

### Work Summary

For GSoC 2019 I've initiated the project nodecloud-cli from scratch and added support for AWS and Google cloud platform and Azure.

nodeloud-cli support following services,
- Compute
- Identity Management
- Network
- Storage

Along with development of CLI, I added documentation and unit tests in every week.
Created tutorials.


### What Covered

- Developed the CLI for compute, identity manamgement, network and storage services.

	1. AWS
		- EC2
		- ECS
		- DynamoDB
		- RDs
		- S3
		- ELB
	2. GCP
		- Compute
		- Datastore
		- Google Cloud DNS
		- Google Cloud Storage

	3. Azure
		- Virtual Machine


- Added unit tests for developed cli.
- Added documentation for developed cli.
- Created nodecloud-cli getting started tutorial.

### What left

- Adding Pretty or beautify option for the cli.
- Potential to add more cloud providers like Digital ocean, Ali cloud.

### Reference

- [AWS and Google Cloud platform comparison](https://cloud.google.com/docs/compare/aws/)
- [AWS JS SDK Documentation](http://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS.html)
- [Google Cloud platform Documentation](https://googlecloudplatform.github.io/google-cloud-node/)