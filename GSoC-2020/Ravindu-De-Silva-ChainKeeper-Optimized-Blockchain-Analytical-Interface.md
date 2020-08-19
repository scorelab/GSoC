# ChainKeeper - Optimized Blockchain Analytical Interface

## Student Info

* Name - Ravindu De Silva
* Email - deravindusilva@gmail.com
* GitHub Profile - https://github.com/Ammoniya
* Medium - https://medium.com/@deravindusilva
* Twitter - https://twitter.com/deravindus

### Project Abstract
ChainKeeper analytic is a bitcoin analysis project for identifying mixing transactions/wallets. Chain keeper analytics made to gather data from truested sources and model them into a graph then run some graph-based machine learning analytics like Node2Vec, Path2Vec, Link predection, etc.  The ultimate goal of the Chainkeeprt analytic is to build an unsupervised graph-based mixing network detecting analytic engine and deploy it with the SCoRe Lab Chain keeper project. 

### [GSoC Project Page](https://summerofcode.withgoogle.com/organizations/6706542746796032/)

### [GSoC Project Proposal](https://drive.google.com/file/d/1OCVJhKlWM0bDbK9efICEh0gBrs9C5NQS/view?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/ChainKeeper-Analytics)

### [GitHub Personal Repo](https://github.com/Ammoniya/ChainKeeper-Analytics)

### [Commits during GSoC 2020](https://github.com/Ammoniya/ChainKeeper-Analytics/commits/master)

### [Project Demo Video]()

### GSoC Blog(s)
[Bitcoin Hunting with SCoRe Lab GSOC 2020](https://medium.com/scorelab/bitcoin-hunting-with-score-lab-gsoc-2020-73037a572f3c) <br>
[Walletexplorer](https://medium.com/scorelab/walletexplorer-e3d4a7adc4c0)

### Work Summary
Chainkeepr analytic is a bitcoin mixing network detecting engine. Since it was the start of the project, the major requirements were to identify some trusted data sources, gather some required amount of data and conduct some graph-based data analysis on top of the data. The project had two phases. One is to gather the data and other one is to build the model. During the GSoC time period, I have discovered some trusted data sources, coded data crawlers, automated crawlers, modeled collected data into a graph, conducted an analysis on top of the modeled graph and built the primary analysis model. 
<br><br><br>
![Untitled Diagram (3)](https://user-images.githubusercontent.com/20130001/90658529-4e34a700-e261-11ea-93bf-b53f0d906350.png)
<br><br><br>
### What Covered
Follow shows the summary of my contribution to the chain keeper analytic during GSoC 2020.
##### Data gathering crawlers
* Created bitcoinabuse and walletexplorer d ata gathering crawlers. [[PR-2]](https://github.com/scorelab/ChainKeeper-Analytics/pull/2)
* Optimized and debugged bitcoinabuse and walletexplorer and created the walletexplorer scan crawler. [[PR-3]](https://github.com/scorelab/ChainKeeper-Analytics/pull/3)
* Containerized BlockSci tool. [[PR-4]](https://github.com/scorelab/ChainKeeper-Analytics/pull/4)
##### Data Analysis
* Analyzed the data (initial analysis of data).  [[PR-6]](https://github.com/scorelab/ChainKeeper-Analytics/pull/6)
* Community Detection Analysis [Domain-Bitcoin Address].  [[PR-7]](https://github.com/scorelab/ChainKeeper-Analytics/pull/7)
* Node classification with Node2Vec [bitcoin address vs domains vs pages] with TSNE clustering [bitcoin address vs domains vs pages].  [[PR-8]](https://github.com/scorelab/ChainKeeper-Analytics/pull/8) 
* Built graph prediction models (node2vec-link-prediction [bitcoin address vs domains vs pages]).  [[PR-9]](https://github.com/scorelab/ChainKeeper-Analytics/pull/9)
* Domain clustering with T-SNE dimension reduction and HC-agglomerative (single, complete, ward, average).  [[PR-11]](https://github.com/scorelab/ChainKeeper-Analytics/pull/11)
* Clustering graph nodes.  [[PR-12]](https://github.com/scorelab/ChainKeeper-Analytics/pull/12)

### What left

### Reference
