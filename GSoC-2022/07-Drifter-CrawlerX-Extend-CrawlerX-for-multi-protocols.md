# CrawlerX - Extend CrawlerX for Multi Protocols

## Student Info
* Name - Chiran Malith Karunasinghe
* Email - chirankarunasinghe3@gmail.com
* GitHub Profile - https://github.com/DrifterKaru

# Project Abstract

Web scraping, commonly referred to as web scraping, is a method of programmatically traversing a collection of web pages and extracting data that is useful for data analysis of web-based data. In the current project, CrawlerX is - distributed extensible scalable web crawling platform: platform that we can use to crawl web URLs in a distributed fashion with different types of protocols. Web scraping, commonly referred to as web scraping, is a method of programmatically traversing a collection of web pages and extracting data, which is useful for data analysis using web-based data. Using a web crawler, you can mine data about a set of products, get lots of textual or quantitative data to use, get data from sites that don't have an official API, or just satisfy your own personal curiosity. However, when using the CrawlerX platform, users may encounter UX issues and feature gaps that are useful for data analysis. Also, such tools will mostly be useful for Darkweb analysis and gathering malicious and criminal records to investigate law enforcement duties. 

![CrawlerX with Tor](https://github.com/leopardslab/CrawlerX/blob/master/resources/Crawlerx_Tor.jpg)


## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/9x4krJ3S)

## [GSoC Project Proposal](https://drive.google.com/file/d/1Ei4Fm_Kpl6m6b4yggwzu1weT7fuYEBwM/view)

## [GitHub Organization Repo](https://github.com/leopardslab/CrawlerX)

## [GitHub Personal Repo](https://github.com/DrifterKaru/CrawlerX)

## [Commits during GSoC 2022](https://github.com/leopardslab/CrawlerX/commits?author=DrifterKaru)

# Work Summary

   Majorly this project covered adding multi protocol support for CrawlerX by integrating Tor Proxy and relevant proxy configurations in Scrapy and other inner components. When a user starts the CrawlerX application executing docker compose command Tor proxy starts default and ready to serve onion crawl requests on demand. Also, with the CrawlerX web application, users can schedule any onion URLs in all the scheduling types that CrawlerX provides by selecting Tor_Onion crawling type. Refer following images for the basic idea of the tasks. Moreover, few useful spiders was added to the Scrapy server that are very important in terms of data analysis and researches.

   
- Web Application Option 
  
    ![CrawlerX - Schedule Job](https://github.com/leopardslab/CrawlerX/blob/master/resources/DarkWeb_Onion_Option.png)

- Tor Proxy
  
    ![Docker Compose](https://github.com/leopardslab/CrawlerX/blob/master/resources/Tor_Proxy_Config.png)


# What Covered

- Integrating Tor Proxy with relevant configurations
- Adding Srapy Tor onion spider
- Adding Scrapy Research Gate spider
- Adding Medium article spider
- Secured endpoints to fetch dark web crawled data
- Schedule crawler jobs for dark web URLs
- Testing Tor onion multi protocol support
- Did relevant database and Celery component level changes
- Update Readme file


# Reference

1. [Tor Project](https://www.torproject.org/)
2. [Docker Compose](https://docs.docker.com/compose/)
