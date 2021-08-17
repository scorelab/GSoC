# CrawlerX Distributed Crawling System

## Student Info
* Name - Sandagomi Pieris  
* Email - npieris73@gmail.com
* GitHub Profile - https://github.com/sandagomipieris

# Project Abstract
The CrawlerX is a platform that we can use for crawling web URLs in different kinds of protocols in a distributed way. Web crawling often called web scraping is a method of programmatically going over a collection of web pages and extracting data which is useful for data analysis with web-based data. With a web scraper, you can mine data about a set of products, get a large corpus of text or quantitative data to play around with, get data from a site without an official API, or just satisfy your own personal curiosity. CrawlerX was a platform designed to run on a VM-based environment with limited functionality. This project extends that limitation to the containerized environments.

![K8s with Helm](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm.png)

## [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5366481539301376)

## [GSoC Project Proposal](https://drive.google.com/file/d/1k8RGMx9kMIpFNBgz9BFh2bnJfyxLujVS/view)

## [GitHub Organization Repo](https://github.com/leopardslab/CrawlerX)

## [GitHub Personal Repo](https://github.com/sandagomipieris/CrawlerX)

## [Commits during GSoC 2021](https://github.com/leopardslab/CrawlerX/commits?author=sandagomipieris)

## Project Overview

1. Pod Deployment

![Pods](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm/helm_1.png)

2. Service Deployment

![Services](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm/helm_2.png)

3. Ingress Deployment

![Ingress](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm/helm_3.png)

4. ConfigMap Deployment

![ConfigMaps](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm/helm_4.png)

# Work Summary

This project mainly focuses on deploying the CrawlerX web platform on Kubernetes. As per the details provided by SCoRe organization mentors, CrawlerX needs to be deployed as an on-demand platform. Therefore, as per the investigations Helm is used to implementing the requirement. Helm helps you manage Kubernetes applications as Charts. Charts are easy to create, version, share, and publish also unpublish. Now users can deploy the CrawlerX on the K8s environment with a single command as follows.

```bash
helm install <RELEASE_NAME> <HELM_HOME> --namespace <NAMESPACE> --dependency-update --create-namespace
```
![Helm Deployment](https://github.com/leopardslab/CrawlerX/blob/master/resources/helm/helm_5.png)

# What Covered

* Add Helm chart for CrawlerX platform
* Add K8s artifacts for VueJS based frontend server deployment
* Add K8s artifacts for Django backend server deployment
* Add K8s artifacts for Celery beat deployment
* Add K8s artifacts for Celery worker deployment
* Add K8s artifacts for Scrapy crawler deployment
* Add MongoDB, RabbitMQ and Elasticsearch deployments as chart dependencies
* Add K8s secret artifacts to pull private images for the pods
* Add ConfigMaps for each deployment
* Configure values.yaml to customize deployment parameters
* Documentation of the K8s deployment
* Testing on Minikube local server
* Testing on Google Kubernetes Engine 

# What left

* Integrate Grafana dashboard

# Reference

1. [Helm](https://helm.sh/)
2. [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine)
