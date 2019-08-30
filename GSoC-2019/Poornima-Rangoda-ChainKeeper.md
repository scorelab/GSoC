# ChainKeeper - Optimized Analytical Interface for ChainKeeper

## Student Info
- Name : Poornima Kavindi Rangoda
- Email : poornima.k.rangoda@gmail.com
- University : Monash University Australia
- GitHub handle : https://github.com/poornimarangoda

### Project Abstract
ChainKeeper Analysis Library is a platform where user can analyse the blockchain data which are the outputs of the ChainKeeper parse. From this implemented ChainKeeper Analysis Libraries users able to retreive Blockchain, Block, Transaction, Input, Output data and Address data by accessing the python library called **chainkeeper_analysis.so**.  

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#4719437733691392)

### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/4547182600912896_1554647600_GSoC_2019-ChainKeeper-Final_proposal.pdf?Expires=1566762011&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=OOpo0J%2F7PrWR13zGlpNKC%2Ft8HFBpUQijT8DnGhX5MmcyQ998sIpiaJolXhZkTPieryuggR7bz0rtwxFjZcXMDF0Tyz8ETM0fTaQZ%2BzhPa96h25P99rHQJHKfrhSmZAOetgSY2m4EWVHwBXLw5VOxYqMoMvy7ZFEH26mrhJXQqB7jefkZkSpAHMG%2BjxpZhCo9B9tK8AmUzBaVSqeSG3mfLrwp%2BG7UENbbKAX4CjMNIkrpeqnTvZae6PCe6eUEaQtZ09iN%2FjbL3%2B9TQ1iSFiVFY9zFw%2BopQAJSiSK%2FYygQbLs0ecSEe%2BRhm9vfo8VwhRKo1H5v81DB4k0srTSVGYz6ug%3D%3D)

### [GitHub Organization Repo](https://github.com/scorelab/ChainKeeper)

### [GitHub Personal Repo](https://github.com/poornimarangoda/ChainKeeper)

### [Commits during GSoC 2019](https://github.com/scorelab/ChainKeeper/pulls?utf8=%E2%9C%93&q=is%3Apr+is%3Aclosed+author%3Apoornimarangoda)

### [Project Wiki](https://github.com/scorelab/ChainKeeper/tree/master/analysis-library/gdoc)

### Work Summary
During the GSoC 2019 I have developed an analytical interface for the blockchain which is useful for the analysis activities doing for the blockchains. Basically it has two types of interfaces. Blockchain data and Addresses.In Blockchain data it contains data classes for Blockchain, Block, Tx, Input and Output. For the Address for the moment there is a Address class. All these classes have defined inside the PYTHON_MODULE method of C++ boost library. From this PYTHON_MODULE we can create a shared library supports to the python. Boost enables to create python data structures in C++. Therefore, library methods can return data which are compatible with python environment. Then this shared python library can be used in Jupyter interface to access the Core Blockchain Data.

### What Covered
- Implementation of the Analysis Library architecture
- Implement the analytical interface for the blockchain dataset
- Implement the analystical interface for the address
- Connect the analytical interface with the output of the parser data
- Optimized data retrieving queries based on performance
- Documentaions of the Analysis Library
- Testing the project

### What left
- Add new methods for the Address class interface 
- Performance evaluation based on the file based system for parser data

### Reference
- [BlockSci Research paper](https://arxiv.org/abs/1709.02489) 
- [Boost C++ Library](https://www.boost.org/doc/libs/1_39_0/libs/python/doc/index.html)
- [C++ Standards](https://www.tutorialspoint.com/cplusplus/cpp_multithreading.htm)
