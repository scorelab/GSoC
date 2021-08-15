# CrawlerX - Extensible, Distributed, Scalable Crawler System

## Student Info
* Name - Beshini Ekanayake  
* Email - beshiniii13@gmail.com
* GitHub Profile - https://github.com/beshiniii

# Project Abstract
Web scraping is usually called web crawling, which is a method of programmatically traversing a collection of web pages and extracting data that is useful for data analysis on web-based data. As of the current project, the CrawlerX is a platform which we can use for crawling web URLs in different kinds of protocols in a distributed way. Web crawling often called web scraping is a method of programmatically going over a collection of web pages and extracting data which is useful for data analysis with web-based data. With a web scraper, you can mine data about a set of products, get a large corpus of text or quantitative data to play around with, get data from a site without an official API, or just satisfy your own personal curiosity. 

![CrawlerX - Architecture Diagram](https://github.com/leopardslab/CrawlerX/blob/master/resources/abstract_architecture.jpg)

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6734219864178688)

## [GSoC Project Proposal](https://drive.google.com/file/d/1Vv7Iwe3wi1Vx48u72aHHV7gI3n7fPMWu/view)

## [GitHub Organization Repo](https://github.com/leopardslab/CrawlerX)

## [GitHub Personal Repo](https://github.com/beshiniii/CrawlerX)

## [Commits during GSoC 2021](https://github.com/leopardslab/CrawlerX/commits?author=beshiniii)

## Project Overview

1. Implemented CrawlerX Dashboard

![Dashboard](https://github.com/leopardslab/CrawlerX/blob/master/resources/dashboard.png)

2. Job Scheduler

![Scheduler](https://github.com/leopardslab/CrawlerX/blob/master/resources/job_schedule.png)

3. [Documentation](https://github.com/leopardslab/CrawlerX/blob/master/README.md)

# Work Summary
For the GSoC 2021, I have improved the current status of the CrawlerX platform which is an extensible, distributed, scalable crawler system for its end-users. Previous it had only one option to schedule a crawl job which is as an instant scheduler. Also, it had multiple limitations since it was implemented in a very complex way. During GSoC 2021 in the abstract, I integrated the Django-celery-beat and worker extensions to the backend server and now it is capable of scheduling jobs in three ways; as instant, as interval and as cron schedulers. Also, it has support to enable disable the running schedule tasks and delete unwanted data from the platform. Also, in the case of previewing data, it supports copy data and downloads data as a JSON option to export crawled data to external usages.

# What Covered

* Integrate Celery Beats to the CrawlerX project to store the periodic task schedule in the database.
* Integrate Celery workers to execute scheduled tasks from the database.
* Integrate RabbitMQ broker as the celery database to store schedule tasks.
* Add API endpoints to schedule crawl jobs.
* Introduce Instant Scheduler to schedule tasks instantly.
* Introduce Interval Scheduler to schedule tasks as period tasks.
* Introduce Cron Scheduler to schedule tasks as cron jobs.
* Add feature to delete running and completed crawl tasks.
* Add feature to disable and enable running schedule tasks.
* Add option to export the crawled data as a JSON file. 
* Improve UI design of the CrawlerX dashboard.
* Add environment variable to configure project.
* Updating docker-composer file to deploy the CrawlerX on Docker.

# What left

* Crawl Tor based URLs.

# Reference

1. [VueJS](https://vuejs.org/)
2. [Celery](https://github.com/celery/django-celery-beat)
