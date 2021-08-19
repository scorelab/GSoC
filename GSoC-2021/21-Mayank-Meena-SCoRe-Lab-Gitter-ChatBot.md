# Gitter-ChatBot

## Student Info

- Name - Mayank Meena
- Email - mayank_m@cs.iitr.ac.in, mayank16meena@gmail.com
- University - Indian Institute of Technology Roorkee
- GitHub Profile - https://github.com/maayami
- LinkedIn profile - https://www.linkedin.com/in/mayankmeina/
- Medium - https://maayamiwrites.medium.com/
- Twitter - [maayamiTweets](https://twitter.com/maayamiTweets)

### Project Abstract

Many open-source contributors face challenges to get started with the community's projects. This project aims to
make a Gitter chatbot for the organization's Gitter channel to help new contributors ﬁnd projects of their skills/
interests. GItter-ChatBot uses gitter-stream-api to listen to all the messages in the gitter channel of a community. It determines the use-cases based on the search techniques that are present in its memory (as python lists/dictonaries/arrays). Gitter RESTful-API integration allows it to communicate with the user.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5570345467117568)

### [GSoC Project Proposal](https://docs.google.com/document/d/1EOwUy7nP-xffy9i3CRqODanFWl-0bi5W-hUK9ywDDHQ/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/leopardslab/Gitter-ChatBot)

### [GitHub Personal Repo](https://github.com/maayami/Gitter-ChatBot)

### Commits during GSoC 2021

- [PR 1](https://github.com/leopardslab/Gitter-ChatBot/pull/4)
- [PR 2](https://github.com/leopardslab/Gitter-ChatBot/pull/6)
- [PR 3](https://github.com/leopardslab/Gitter-ChatBot/pull/8)
- [PR 4](https://github.com/leopardslab/Gitter-ChatBot/pull/10)
- [PR 5](https://github.com/leopardslab/Gitter-ChatBot/pull/12)
- [PR 6](https://github.com/leopardslab/Gitter-ChatBot/pull/14)
- [PR 7](https://github.com/leopardslab/Gitter-ChatBot/pull/15)
- [PR 8](https://github.com/leopardslab/Gitter-ChatBot/pull/18)
- [PR 9](https://github.com/leopardslab/Gitter-ChatBot/pull/20)
- [PR 10](https://github.com/leopardslab/Gitter-ChatBot/pull/22)
- [PR 11](https://github.com/leopardslab/Gitter-ChatBot/pull/23)
- [PR 12](https://github.com/leopardslab/Gitter-ChatBot/pull/24)
- [PR 13](https://github.com/leopardslab/Gitter-ChatBot/pull/25)
- [PR 14](https://github.com/leopardslab/Gitter-ChatBot/pull/27)

### Project Demo Video

- YouTube: https://www.youtube.com/watch?v=Z5A6oj88Yp0
- Google drive: https://drive.google.com/file/d/1qjrLzaTwPoNobzOmU1krzzrQ8yYxbGTL/view?usp=sharing

### GSoC Blog

- [GSoC’21 | Score Lab — A fable on the community bonding period](https://medium.com/leopards-lab/gsoc21-score-lab-a-new-chapter-19a56bec5deb)
- [GSoC’21 with Score Lab | Gitter ChatBot | Phase-1](https://medium.com/leopards-lab/gsoc21-with-score-lab-gitter-chatbot-phase-1-55bc257b1fb1)
- [GSOC 2021 | Score Lab: Unit testing and Code quality](https://medium.com/leopards-lab/gsoc-2021-score-lab-unit-testing-and-code-quality-4881ed1dfad4)
- [GSoC 2021 | Score Lab: Database 'nd da bot](https://medium.com/leopards-lab/gsoc-2021-score-lab-database-nd-da-bot-f26491d18cc9)
- [GSoC 2021 | Score Lab: Final Touches](https://medium.com/leopards-lab/gsoc-2021-score-lab-final-touches-54d11eb0475a)
- [GSoC 2021 | Score Lab : Gitter-ChatBot da Deployment](https://medium.com/leopards-lab/gsoc-2021-score-lab-gitter-chatbot-da-deployment-75d0a0d3b5af)

### Work Summary

**Module Level Implementation of the features**

Worked on connecting a python script to a Gitter channel (used python-gitterpy library). Used Gitter-stream API to liten to all the chat messages.
Created modules to perform all the features like:
- main.py module as the main body of the Gitter-ChatBot, it is responsible for the gitter-channel communication (listen and send messages).
- data_extraction module to extract all the necessary information from a mesage. It searches for skills/Interests of the user.
Created a MongoDB Atlas server for database queries and storage. It stores community projects `(_id, tags[], name, github-link, gitter-link, good-first-issues)`.
- database module deals with the database connection(MongoDB) and fetching the project list from Github-API and updating the database with it.
Worked on the response generation feature that responds to the gitter-channel. Written unit-tests for the data_extraction module. Written a fully-fledged Documentation for the project.

### What Covered

Implemented four use-cases:
1. Welcoming a new user, when they send their first message. If message does not contain any skill/interest of the user, ask the user to provide the same.

![image](https://user-images.githubusercontent.com/55585868/129679929-c3d4b620-9771-4c04-a561-a8af0feb2bd8.png)

2. Query the database for the given information and fetch a list of projects.

![image](https://user-images.githubusercontent.com/55585868/129680464-1c67acfb-3efa-4e6b-852b-681433776c52.png)

3. Created a quick help guide for the ChatBot.

![image](https://user-images.githubusercontent.com/55585868/129680155-0df1749b-8c71-4377-b23a-8ee9aa7f68e8.png)

4. An existing user can aslo ask for a project list.

![image](https://user-images.githubusercontent.com/55585868/129680074-1824bf41-bd67-4aa0-b368-5dd46fe3ea07.png)


**Github Issues**

- [Issue 1](https://github.com/leopardslab/Gitter-ChatBot/issues/1)
- [Issue 2](https://github.com/leopardslab/Gitter-ChatBot/issues/2)
- [Issue 3](https://github.com/leopardslab/Gitter-ChatBot/issues/3)
- [Issue 4](https://github.com/leopardslab/Gitter-ChatBot/issues/13)
- [Issue 5](https://github.com/leopardslab/Gitter-ChatBot/issues/5)
- [Issue 6](https://github.com/leopardslab/Gitter-ChatBot/issues/16)
- [Issue 7](https://github.com/leopardslab/Gitter-ChatBot/issues/7)
- [Issue 7](https://github.com/leopardslab/Gitter-ChatBot/issues/17)
- [Issue 8](https://github.com/leopardslab/Gitter-ChatBot/issues/19)
- [Issue 9](https://github.com/leopardslab/Gitter-ChatBot/issues/9)
- [Issue 11](https://github.com/leopardslab/Gitter-ChatBot/issues/11)
- [Issue 12](https://github.com/leopardslab/Gitter-ChatBot/issues/21)
- [Issue 13](https://github.com/leopardslab/Gitter-ChatBot/issues/26)

### What left

All the project milestones have been achieved and below improvements can be made to the project:
- Fixing [bug](https://github.com/leopardslab/Gitter-ChatBot/issues/16) regarding data_extraction module. 

### References

- [Gitter-ChatBot's Notion Book](https://rattle-clavicle-0cc.notion.site/GSoC-21-Gitter-ChatBot-f0ba6af8720a42b89b500c2302de8d15)
- [python-unittest library](https://www.journaldev.com/15899/python-unittest-unit-test-example)
- [Python Linting](https://www.pylint.org/)
- [Unittesting Tutorial](https://www.datacamp.com/community/tutorials/unit-testing-python)
- [Code sStructure of a Python Directory](https://docs.python-guide.org/writing/structure/)
- [Writing setup.py file for a python package](https://github.com/kennethreitz/setup.py)
