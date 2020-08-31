# CrawlerX - Extensible, Distributed, Scalable Crawler System

## Student Info

* Name - Poornima Rangoda	
* Email - poornima.k.rangoda@gmail.com
* GitHub Profile - https://github.com/poornimarangoda
* Medium - https://medium.com/@poornimar.blogger

### Project Abstract
The CrawlerX is a platform which we can use for crawl web URLs in different kind of protocols in a distributed way. Web crawling often called web scraping is a method of programmatically going over a collection of web pages and extracting data which useful for data analysis with web-based data. With a web scraper, you can mine data about a set of products, get a large corpus of text or quantitative data to play around with, get data from a site without an official API, or just satisfy your own personal curiosity.

![CrawlerX - Architecture Diagram](https://raw.githubusercontent.com/leopardslab/CrawlerX/master/resources/architecture_diagram.jpg)

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4546083851599872)

### [GSoC Project Proposal](https://drive.google.com/file/d/1ys3cfM00_1rXg-xWPqQbDuuleIzkZW18/view)

### [GitHub Organization Repo](https://github.com/leopardslab/CrawlerX)

### [GitHub Personal Repo](https://github.com/poornimarangoda/CrawlerX)

### [Commits during GSoC 2020](https://github.com/leopardslab/CrawlerX/pulls?q=is%3Apr+is%3Aclosed+author%3Apoornimarangoda)

### [GSoC Blog]
* Story 1 - [Link](https://medium.com/scorelab/gsoc-with-scorelab-2020-story-01-b845ebc190b8)
* Story 2 - [Link](https://medium.com/@poornimar.blogger/gsoc-with-scorelab-2020-story-02-970ddeba2dc8)

### Work Summary
For the GSoC 2020, I have implemented the CrawlerX platform which is an extensible, distributed, scalable crawler system for the end-users. With this platform, now users can simply crawl any kind of URL as he desired. In this platform, I have implemented 3 main spiders for crawling mechanisms. What users need to do is, just log in to the system, create a project using the intuitive user interface and schedule the crawl job by adding required URLs. Also, the CrawlerX platform is capable to preview what are the created projects by users, corresponding jobs and the results of the scheduled jobs with its status. Additionally, users can see the crawled data with this platform just from one click.

### What Covered
* User login with Firebase authentication and authorization.
* Project creation for Crawling jobs.
* Crawling job scheduling.
* Backend integration with Django REST APIs.
* Message broker functionality for extensibility with RabbitMQ. 
* Job scheduling capability with Scrapy.
* Integrate data storing functionality with MongoDB.
* Platform wise centralized logs/query analysis with ElasticSearch. 
* Crawled data previewing. 
* UI for the CrawlerX platform with VueJS. 

### What left
* Upload crawling URLs from files.
* Kubernetes artifacts.

### Reference
1. [Scrapy](https://scrapy.org/)
2. [VueJS](https://vuejs.org/)
