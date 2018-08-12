# Project Name
ChainKeeper

## Student Info
- <b>Name</b>: Sajitha Gimash Hikkaduwa Liyanage
- <b>Email</b>: [sajithaliyanage@gmail.com](mailto:sajithaliyanage@gmail.com)
- <b>University</b>: University of Colombo School of Computing, Sri Lanka
- <b>GitHub Profile</b>: [https://github.com/sajithaliyanage](https://github.com/sajithaliyanage)
- <b>LinkedIn Profile</b>: [https://www.linkedin.com/in/sajithaliyanage](https://www.linkedin.com/in/sajithaliyanage)

### Project Abstract
ChainKeeper is a web application to explore and analyze block-chain data for users. It connects with BlockSci which is a tool support for explore and analyse the blockchains. ChainKeeper contains REST API service to get details from blockchains with more additional features. Technical or non-technical users can explore or retrieve blockchain data from ChainKeeper to their need. The main objective of this project is to design and implement a web based application for ChainKeeper using React. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5938458648903680)

### [GSoC Project Proposal](https://docs.google.com/document/d/10nTSVxTE8ZOjnqaSvFG-icPl-lSD1kT0YEA_UtN4I_I/edit?usp=sharing)

### GitHub Organization Repo
- [ChainKeeper Repo](https://github.com/scorelab/ChainKeeper)  - Web based application to explore and analyze block-chain 
- [ChainCleaner Repo](https://github.com/scorelab/chain-cleaner) - Sub feature of ChainKeeper for taint analysis of Bitcoin

### [GitHub Personal Repo](https://github.com/sajithaliyanage/ChainKeeper)

### Commits during GSoC 2018
- [ChainKeeper Repo](https://github.com/scorelab/ChainKeeper/commits?author=sajithaliyanage)
- [ChainCleaner Repo](https://github.com/scorelab/chain-cleaner/commits?author=sajithaliyanage)

### [Project Wiki](https://github.com/sajithaliyanage/ChainKeeper/wiki)

### GSoC Blog
- [GSoC 2018 Journey with SCoRe Lab — EPI 1](https://medium.com/@sajithaliyanage/gsoc-2018-journey-with-score-lab-part-1-b6a71c046dd7)
- [GSoC 2018 Journey with SCoRe Lab — EPI 2](https://medium.com/@sajithaliyanage/gsoc-2018-journey-with-score-lab-epi-2-d6cbd5371526)
- [GSoC 2018 Journey with SCoRe Lab — EPI 3](https://medium.com/@sajithaliyanage/gsoc-2018-journey-with-score-lab-epi-3-ce0e87f94793)
- [GSoC 2018 Journey with SCoRe Lab — EPI 4](https://medium.com/@sajithaliyanage/gsoc-2018-journey-with-score-lab-epi-4-ba85c6272c8e)

### Work Summary
For the GSoC 2018, I have implemented two main web based tool to explore blockchains. First one is ChainKeeper which is a web based application to explore and analyze block-chain and the second one is Chain-Cleaner which is a sub tool of ChainKeeper for taint analysis of Bitcoin.

##### 1.0 ChainKeeper
ChainKeeper is a web application to explore and analyze block-chain data for users. It is a web-based application for blockchain developers who are looking to interact with BlockSci to analyse the blockchain data in blockchains. And also ChainKeeper contains separate REST API for getting blockchain data easily. ReactJs and firebase are used to develop the web application and python flask used to develop the REST API.

<b>Features</b>
- Users can sign up or sign in to the ChainKeeper
- Can latest block data in blockchain
- Can view block data using block height
- Can view block data using block hash
- Can view tx data using tx hash
- Can get data from REST endpoints
- Can connect BlockSci with ChainKeeper
- Chain-Kleaner - Taint Analysis platform

##### 2.0 Chain-Cleaner
Chain-Cleaner is a web application to analyse tainted transactions and inputs from the bitcoin blockchain. Users can add heists into the chain-cleaner and those data are used for analyse to find tainted inputs. ReactJs and firebase are used to develop the web application and python used to develop cronjob of memory pool data.

<b>Features</b>
- Users can sign up or sign in to the chain-cleaner
- Can view live memory pool data
- Can view tainted memory pool tx if exists
- Can add new heist
- Can view existing heists

### What Covered
Completed the all of the above mentioned tasks during the GSoC period. Addition to that following thing are covered.
- Testing REST APIs
- Documentaions

### What left
- Tagging transactions
- Analyze tainted transactions with policies
- Adding more REST APIs

### Reference
1. [ReactJs Documentation](https://reactjs.org/docs/hello-world.html)
2. [Firebase Documentation](https://firebase.google.com/docs/)
3. [BlockSci Research Paper](https://arxiv.org/abs/1709.02489)
4. [BlockSci Documentation](https://citp.github.io/BlockSci/index.html)


