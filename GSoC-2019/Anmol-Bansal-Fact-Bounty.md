# Fact Bounty

## Student Info
- Name: Anmol Bansal
- Email: abansal@ec.iitr.ac.in
- University: Indian Institute of Technology Roorkee, India
- GitHub Profile: https://github.com/anmolbansal1
- LinkedIn Profile: https://www.linkedin.com/in/anmol-bansal-557b05149/

### Project Abstract
The Fact-Bounty project is a crowd-driven fact-checking platform. Fact-Bounty tries to minimise this chaos by spreading awareness among people on the authenticity of a news item.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5027395176759296)

### [GSoC Project Proposal](https://docs.google.com/document/d/1UBCcAJQz4i5z3QLdfnBKEj9wxNtIzrhiRLMWp47z-eA/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/fact-Bounty)

### [GitHub Personal Repo](https://github.com/anmolbansal1/fact-Bounty)

### [Commits during GSoC 2018](https://github.com/scorelab/fact-Bounty/commits?author=Anmolbansal1)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/scorelab/fact-Bounty/wiki)

### [GSoC Blog](http://GSoCBlog)

### Work Summary
For the GSoC 2019, I've worked on flask API and scrapy crawlers of this project.
 - Refactored the flask server to make it more scalable and more consistent
 - Restructured the API to make it easier to add more features to it later
 - Re-instantiated crawlers project and write crawlers for 13 news websites
 - Set elasticsearch pipeline to plug all fetched data from crawlers directly to database
 - Add scheduler feature to scrapy to allow crawlers to run after a regular period
 - Add system to only crawl today's news from websites
 - Add SMTP server to the application to allow mailing and use contact_us form
 - Add new env variables to flask app to make it more scalable
 - Implement GitHub pre-commit hook in the flask to allow code convention consistency in project
 - Update flask utilization of access token to make API more flexible
 - Made the flask server to utilize refresh tokens and new routes corresponding to it
 - Improve error handling of various routes
 - Create new voting API utility to allow users to vote news articles
 - Add new routes fetch particular story and search among stories
 - Change date column format in crawlers to allow kibana to generate visualizations in kibana
 - Add new script to run all crawlers simultaneously

### What Covered

### What left
Adding the ability to automtically cluster fake news with the help of machine learning techniques.

### Reference
- [API Documentation | Elasticsearch Python](https://elasticsearch-py.readthedocs.io/en/master/)
- [Scrapy Documentation](https://docs.scrapy.org/en/latest)
