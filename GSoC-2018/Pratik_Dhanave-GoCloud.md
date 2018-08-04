# GoCloud
## Student Info
* Name - Pratik Dhanave
* Email - i.pratikdhanave@gmail.com
* GitHub profile - https://github.com/PratikDhanave


### Project Abstract
gocloud is a standard library for Go that abstracts away differences among multiple cloud providers. Developing golang package for interacting with Google cloud,AWS, Digi Ocean, Ali Cloud using a unified API.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6643006694752256)

### [GSoC Project Proposal](https://docs.google.com/document/d/1a1J5kYc1CtNCTpXCj2JMcAqXsMaMVNUF8iajTEiggO0/edit)

### [GitHub Organization Repo](https://github.com/cloudlibz/gocloud)

### [GitHub Personal Repo](https://github.com/PratikDhanave/gocloud)

### [Commits during GSoC 2018](https://github.com/PratikDhanave/gocloud/commits/awsserverlesslambada-v2)

### [Project Demo Video](https://www.youtube.com/playlist?list=PLOdfztY25UNnxK_0KRRHSngJIyVLDKZxq&disable_polymer=true)

### [Project Wiki](https://github.com/cloudlibz/gocloud/wiki)

### [GSoC Blog](https://medium.com/gocloud)

### Work Summary
For GSoC 2018 I have extended the project support for AWS and Google cloud platform (GCP).

Support for following services were added,
- Serverless
- Database
- Machine Learning
- Analytics
- Notification Service
- Stream Data Processing
- for authentication with AWS cloud I implemented signature-version-4 get method  and signature-version-4 with authetication header method.
- for authentication with Google cloud I implemented OAuth client and  service account authentication method.

Along with development of APIs, I added documentation and unit tests.
Created tutorial series.

### What Covered

- Developed APIs for Serverless, Database, Machine Learning, Analytics, notification and stream data processing.

	1. AWS
		- lambada
		- Amazon DynamoDB
		- Amazon Machine Learning
		- Amazon Redshift 	
		- Amazon Simple Notification Service
    - Amazon Kinesis

	2. GCP
		- Google Cloud functions
		- Google Cloud Bigtable
		- Google Machine Learning Engine
		- BigQuery
		- Cloud Pub/Sub
    - Cloud Dataflow


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
