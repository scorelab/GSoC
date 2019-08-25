# ChainKeeper - Optimized Bitcoin blockchain parser for memory constrained devices

## Student Info
  * Name - Hansika Perera
  * Email - madhuhanz@gmail.com
  * University - Sri Lanka Institute of Information Technology
  * GitHub profile - https://github.com/HansikaPerera
  
### Project Abstract
Bitcoin blockchain is a huge data structure with 180+GB in size. Due to this huge size, available Bitcoin parsers take several hours to parse the entire blockchain. As an example, BlockSci parser takes 11 hours with an 8GB cache. Because of that most of the available Bitcoin parsers are inefficient on memory constrained devices. The goal of this project is to design and implement a Bitcoin parser(may support forks of Bitcoin as well) which can use available memory efficiently to reduce blockchain parsing time on memory constrained devices.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5470681267961856)

### [GSoC Project Proposal](https://storage.googleapis.com/summerofcode-prod.appspot.com/gsoc/core_project/doc/5465564485517312_1554783375_Chainkeeper.pdf?Expires=1566843514&GoogleAccessId=summerofcode-prod%40appspot.gserviceaccount.com&Signature=bMqeoHjam480vGM3EI4eUAHMM9AvsDlLe6R2AcWkyT%2FeZFNWml2DQ%2Bg%2BW%2FO6h%2BkfIh1Cpx9lI5COw2R6Jd%2FjtEGNKqSw%2BdimFgdP652125jVhapk3B1XObB%2Fcw8kh8qjXgF%2F2Lcb%2FZfPSopc%2BdUNsL8XN3ZOhn5OIwQBmM2LZOlQ2kHn8J8z13p8xeVqXhgNjKCvuK10Evk6Kzfj0zamuewAk6JeCwkNvn9%2BSUVEghtXOeibXgpH8x91hHngGS7X6RPPTczUqJ6XxLxeD2rxFQJeIolPChsli%2BbJU810bdg3aTcg%2FAXPVYH%2Fh2VQ2zCNiMw0HT0hlD8dhnGuNL8jRw%3D%3D)

### [GitHub Organization Repo](https://github.com/scorelab/ChainKeeper)

### [GitHub Personal Repo](https://github.com/HansikaPerera/ChainKeeper)

### [Commits during GSoC 2019](https://github.com/scorelab/ChainKeeper/commits?author=HansikaPerera)

### [Project Wiki](https://github.com/scorelab/ChainKeeper/blob/master/parser/README.md)

### Work Summary
In GSoC 2019 I was working on analysing limitations of existing blockchain parsers and develop a solution capable of overcoming said limitations. This was more of a research project where I had to work with different cryptocurrencies and respective parsers to find outperformance limitations and causes. I have been able to discover that this performance limitation is caused by memory constraints. 

In GSoC 2019 I was working on analysing limitations of existing blockchain parsers and develop a solution capable of overcoming said limitations. This was more of a research project where I had to work with different cryptocurrencies and respective parsers to find outperformance limitations and causes. I have been able to discover that this performance limitation is caused by memory constraints. 

The bitcoin blockchain is a huge data structure which is 200+GB. When parsing this data structure in a memory-constrained environment it heavily uses the swapping on the same data which causes an unnecessary number of IO operations which increases exponentially as available memory becomes lesser.

In my project, I address this problem by designing and implementing a blockchain parser which uses partial memory mapping which minimizes the number of IO operations.

I have completed the implementation of blockchain parser which can parse Bitcoin blockchain and other forks of Bitcoin. Implementation has been done with C++, Boost and several external libraries. Furthermore, indices and data are stored in different DBs to optimize the performance of the parser. This has been tested on memory-constrained environments and obtained satisfactory results. 

### What Covered
* Analyse existing Bitcoin blockchain parsers for possible performance limitations
* Design and implement blockchain parser to support Bitcoin and other forks of Bitcoin
* Test the implementation
* Documentaions of the parser

### What left
* Eavluate the performance of the parser interms of speed and time taken to parse the Bitcoin blockchain
* Compare the performance against existing Bitcoin blockchain parsers
* Try parser with different forks of Bitcoin such as LiteCoin, NameCoin etc.

### Reference
* https://bitcoin.org/bitcoin.pdf
* https://github.com/facebook/rocksdb/tree/master/include/rocksdb
* https://github.com/boostorg/boost/wiki/Getting-Started
* https://litecoin.info/index.php/Main_Page
* https://z.cash/the-basics/
