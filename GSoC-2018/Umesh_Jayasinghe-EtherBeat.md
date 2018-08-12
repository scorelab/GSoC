# Project Name
EtherBeat - Optimize block extracting mechanism in EtherBeat

## Student Info
* <b>Name</b> : Umesh Prabushitha Jayasinghe
* <b>University</b> : University of Colombo School of Computing, Sri Lanka.
* <b>Email</b> : [prabushitha@gmail.com](mailto:prabushitha@gmail.com)
* <b>Github</b> : [https://github.com/prabushitha](https://github.com/prabushitha)
* <b>Linkedin</b> : [https://www.linkedin.com/in/prabushitha](https://www.linkedin.com/in/prabushitha)

### Project Abstract
EtherBeat is an Ethereum blockchain analyzer. It provides a set of functions which can be used to analyze blockchain blocks, transactions and other related data. Apart from basic blockchain access operations, Etherbeat provides the ability to custom query on the blockhain. For an example, you can get a list of transactions related to a ethereum account address. Nested queries are also supported. Example scenario would be, you can list only the transactions to a specific account by a given sender address. 


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4657178368016384)

### [GSoC Project Proposal](https://docs.google.com/document/d/1Rp6A-0a-M2xuGclFYEJJLabsgBy3uHcRIorSJ7b7Duk/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/EtherBeat)

### [GitHub Personal Repo](https://github.com/prabushitha/EtherBeat)

### [Commits during GSoC 2018](https://github.com/prabushitha/EtherBeat/commits/parser)

### [Project Demo Video](http://LinkToDemoVideo)

### [Project Wiki](https://github.com/prabushitha/EtherBeat/wiki)

### GSoC Blogposts
- [GSoC 2018 Stories 01: Into the project EtherBeat](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-into-the-project-etherbeat-2112e85b75ae)
- [GSoC 2018 Stories 02: Parse Ethereum Raw Blocks](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-parse-ethereum-raw-blocks-34bf13116552)
- [GSoC 2018 Stories 03: Recover sender from ethereum transaction](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-03-recover-sender-from-ethereum-transaction-41b38d97c56f)
- [GSoC 2018 Stories 04: Analyzable blockchain structure](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-04-analyzable-blockchain-structure-7342c05435cc)
- [GSoC 2018 Stories 05: SQLite multiple insertions (batch insertions)](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-05-sqlite-multiple-insertions-batch-insertions-eeaa13d9522b)
- [GSoC 2018 Stories 06 : Producer-Consumer Architecture of EtherBuilder](https://medium.com/@umeshprabushithajayasinghe/gsoc-2018-stories-06-producer-consumer-architecture-of-etherbuilder-804044d60e64)

### Work Summary

For GSoC 2018, I've implemented two tools from the scratch which facilitate ethereum blockchain analysis. First tool (<b>EtherExtractor</b>) is to extract blockchain data and the next tool (<b>EtherBuilder</b>) is to parse the blockchain into an analyzable structure. Both tools has been implemented using C++.

##### 1.0 EtherExtractor
A tool which connects to the leveldb ethereum blockchain (currently supports Geth synced chain) and extract block related information. This doesn't need any RPC or IPC endpoints to be active, it directly acccess leveldb to get information. EtherExtractor is an independent tool, which can be extended to applications which needs to access blockchain.

<b>Features</b>
- API which provides direct access to the blockchain
- No network communication overhead
- Ability to extended into a standalone application
- Ability to use as a library
- Fast since this focus only read operations

##### 2.0 EtherBuilder
Tool to store ethereum blockchain in order to support analysis. SQLite database and Rocksdb has been used. Producer-consumer architecture has been used to efficiently manage cpu and memory in order to store data in sqlite and rocksdb. 

### What Covered

- Raw leveldb blockchain access (includes preparation of keys, byte manipulation)
- RLP encoding and decoding
- Public key extraction from a transaction
- Extractor module access following data.
  - block (by number, by hash)
  - block header 
  - transaction (by hash)
  - transaction receipt (by hash)
- Storing of blocks (header+body), transactions, transaction receipts, transactions related to blocks, transactions by addresses
- Indexing of blocks, transactions, transaction receipts, addresses
- Mapping between hashes and indexes
- Exporting EtherExtractor as a library
- Dockerization of EtherBuilder (Deployed and tested the functionalities in a GCP VM)
- Adhere into Google C++ Coding Standards
- Unit tests for EtherExtractor using googletest framework
- Support for geth synced blockchain
- Documentation

### What left

- Access states using merkel patricia tree (this can be used to check balance of a particular address at a given block height)
- Python interface to access stored data 
- Testing the functionality with the full blockchain node
- Checking the capability of adapting to blockchains synced with parity and cpp-ethereum client

### Reference
1. [Domain knowledge I Gathered to Start EtherBeat Project](https://drive.google.com/file/d/1WISuolSL1vuYpJlDcxR5m3fO7g9xdX1g/view)
2. [Google C++ Coding Standards](http://google.github.io/styleguide/cppguide.html)
3. [Geth - Ethereum Client](https://github.com/ethereum/go-ethereum)
4. [Ethereum Yellow Paper](https://ethereum.github.io/yellowpaper/paper.pdf)
5. [Merkel Patricia Tree](https://github.com/ethereum/wiki/wiki/Patricia-Tree)
6. [Ethereum Glossary](https://github.com/ethereum/wiki/wiki/Glossary)
