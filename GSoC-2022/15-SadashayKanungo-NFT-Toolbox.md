# NFT-Toolbox
## Student Info
- Name : Sadashay Kanungo
- Email : sadashay01@gmail.com
- Profiles : [Github](https://github.com/SadashayKanungo) | [Medium](https://medium.com/@sadashay) | [LinkedIn](https://www.linkedin.com/in/sadashay-kanungo-22a4321a0)

# Project Abstract
Non Fungible Tokens can provide many creators a platform to monetize their digital creations. 
However the understanding of Web3 technologies like Smart Contracts, Transactions, Wallets, Gas etc required to utilize this technology becomes a barrier for them.

NFT-Toolbox is a new NPM package that provides simplistic implementations for the various functionalities that are a part of NFT creation process. 
NFT-Toolbox makes the life of Web3 developers easier and also enables Web2 developers to seamlessly incorporate Web3 functionalities in their projects. 
The applications built using NFT-Toolbox will empower creators to monetize their creations without having to worry about the technicalities of Web3.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/2PHsoS0l)

## [GSoC Project Proposal](https://docs.google.com/document/d/1T1LRM2bZ5UEtg9G3WQqPlc78zAT4rzZ1irwQJPR_e1w/edit?usp=sharing)

## [GitHub Organization Repo](https://github.com/scorelab/NFT-Toolbox)

## [GitHub Personal Repo](https://github.com/SadashayKanungo/NFT-Toolbox)

## [Commits during GSoC 2017](https://github.com/scorelab/NFT-Toolbox/commits/main?author=SadashayKanungo)

## [Project Demo Video](https://www.youtube.com/watch?v=tU_mQwra5vM)

## [Project Tracker During GSoC](https://roomy-submarine-95b.notion.site/GSoC-22-Progress-Report-c8d43182fcda4bfbb88f78d229e89a3f)

## GSoC Blogs
- [GSoC’22 Week 0: Early Initiations](https://medium.com/scorelab/gsoc22-week-0-the-kick-off-929bcac6e424)
- [GSoC’22 Week 1 & 2: Colorful Permutations](https://medium.com/scorelab/gsoc22-week-1-2-colorful-permutations-4bd5b6fc4b82)
- [GSoC’22 Week 3 & 4: Contractual Configurations](https://medium.com/scorelab/gsoc22-week-3-4-contractual-configurations-9a1e33466ec5)
- [GSoC’22 Week 5 & 6: Tokenized Creations](https://medium.com/scorelab/gsoc22-week-5-6-tokenized-creations-59faac113688)
- [GSoC’22 Week 7 & 8: Final Modifications](https://medium.com/scorelab/gsoc22-week-7-8-final-modifications-2782c42f7dc3)
- [GSoC’22 Week 9 & 10: Comprehensive Documentations](https://medium.com/scorelab/gsoc22-week-9-10-comprehensive-documentations-8e6379643c3e)
- [GSoC’22 Week 11 & 12: Imminent Conclusions](https://medium.com/scorelab/gsoc22-week-11-12-imminent-conclusions-365baa563940)

# Work Summary
GSoC'22 was the inception of NFT-Toolbox. Starting from scratch, a total of five functionalities have been implemented.
Here is the overview of the functionalities:
- Generate Functionality
  - Generating Images and Metadata files for an NFT Collection from Layer Images
  - Useful for creating large collections, most popular technique to create Profile Picture Projects
  - Implementation inspired by the Hashlips Art Engine, popular tool in the NFT community for generating NFT collections
- Upload Functionality
  - Uploading Asset and Metadata files to multiple decentralized file storage platforms
  - Supported platforms: NFT.storage, Pinata, Storj, Infura and Arweave
- Drafting Functionality
  - Programatically generating Solidity Smart Contracts for NFTs
  - Implemented using Open Zeppelin Wizard
- Deploy Functionality
  - Deploying Smart Contracts to Ethereum compatible blockchain networks
  - Implemented using Ethers.js
- Interact Functionality
  - Interacting with Smart Contracts on Ethereum compatible blockchain networks
  - Implemented using Ethers.js

The project has been structured using a Class based approach and is written completely in Typescript.

Unit tests have been included for each class. Mocha, Chai, Sinon, mock-fs and nock have been used to implement the tests.
Example scripts have also been provided for each functionality.

A comprehensive documentation has been created for the project describing all functionalities and complete with examples and guides.
Docusaurus has been used as the documentation generation tool.

## Issues Created
1. Initialize Boilerplate for Typescript Package [(#4)](https://github.com/scorelab/mint-NFT/issues/4)
2. Create Collection class with Generate method [(#5)](https://github.com/scorelab/mint-NFT/issues/5)
3. Create IPFS interface and the classes implementing it [(#6)](https://github.com/scorelab/mint-NFT/issues/6)
4. Create Contract class with Write method [(#7)](https://github.com/scorelab/mint-NFT/issues/7)
5. Add Deploy method to Contract Class [(#8)](https://github.com/scorelab/mint-NFT/issues/8)
6. Create NFT Class [(#9)](https://github.com/scorelab/mint-NFT/issues/9)
7. Add Interaction methods to Contract class [(#10)](https://github.com/scorelab/mint-NFT/issues/10)
8. Create Marketplace Interface and the classes implementing it [(#11)](https://github.com/scorelab/mint-NFT/issues/11)
9. Documentation for the package [(#12)](https://github.com/scorelab/mint-NFT/issues/12)
10. User Guide [(#13)](https://github.com/scorelab/mint-NFT/issues/13)

## Pull Requests Created
| Pull Request | Link | Linked Issues |
|---|---|---|
| Initialized Project, Created Collection Class, Added Examples and Tests for it | https://github.com/scorelab/NFT-Toolbox/pull/14 | [(#4)](https://github.com/scorelab/mint-NFT/issues/4), [(#5)](https://github.com/scorelab/mint-NFT/issues/5)
| Created IPFS Abstract Class and Five Service Classes Extending it | https://github.com/scorelab/NFT-Toolbox/pull/15 | [(#6)](https://github.com/scorelab/mint-NFT/issues/6)
| Created Contract Class with Draft, Deploy and Mint Methods | https://github.com/scorelab/NFT-Toolbox/pull/16 | [(#7)](https://github.com/scorelab/mint-NFT/issues/7), [(#8)](https://github.com/scorelab/mint-NFT/issues/8), [(#10)](https://github.com/scorelab/mint-NFT/issues/10)
| Created Pinata and NFTstorage classes | https://github.com/scorelab/NFT-Toolbox/pull/18 | [(#6)](https://github.com/scorelab/mint-NFT/issues/6)
| Created Storj and Infura Classes | https://github.com/scorelab/NFT-Toolbox/pull/19 | [(#6)](https://github.com/scorelab/mint-NFT/issues/6)
| Created Arweave class | https://github.com/scorelab/NFT-Toolbox/pull/20 | [(#6)](https://github.com/scorelab/mint-NFT/issues/6)
| Created Contract Class with Draft method | https://github.com/scorelab/NFT-Toolbox/pull/21 | [(#7)](https://github.com/scorelab/mint-NFT/issues/7)
| Added Deploy and Interaction methods to Contract Class | https://github.com/scorelab/NFT-Toolbox/pull/22 | [(#8)](https://github.com/scorelab/mint-NFT/issues/8), [(#10)](https://github.com/scorelab/mint-NFT/issues/10)
| Added Documentation with Examples and Guides | https://github.com/scorelab/NFT-Toolbox/pull/23 | [(#12)](https://github.com/scorelab/mint-NFT/issues/12), [(#13)](https://github.com/scorelab/mint-NFT/issues/13)
| Sadashay Branch | https://github.com/scorelab/NFT-Toolbox/pull/24 |  |
| Final Changes | https://github.com/scorelab/NFT-Toolbox/pull/25 |  |


# What is Covered
- Project Initialization and Structure
- Generate Functionality
- Upload Functionality
- Draft Functionality
- Deploy Functionality
- Interact Functionality
- Documentation Project

# What is Left
- Marketplace Functionality: Posting minted NFTs to multiple marketplace platforms for Sale and Auction
- Logo for the package

# References
- Hashlips Art Engine - https://github.com/HashLips/hashlips_art_engine
- Pinata - [https://www.npmjs.com/package/@pinata/sdk](https://www.npmjs.com/package/@pinata/sdk)
- NFT.storage - [https://nft.storage/docs/client/js/](https://nft.storage/docs/client/js/)
- Storj - [https://docs.storj.io/dcs/how-tos/storj-ipfs-pinning-service-beta/](https://docs.storj.io/dcs/how-tos/storj-ipfs-pinning-service-beta/)
- Infura - [https://docs.infura.io/infura/networks/ipfs](https://docs.infura.io/infura/networks/ipfs)
- Arweave (Bundlr) - [https://docs.bundlr.network/docs/client/js](https://docs.bundlr.network/docs/client/js)
- Open Zeppelin Wizard - [https://www.npmjs.com/package/@openzeppelin/wizard](https://www.npmjs.com/package/@openzeppelin/wizard)
- Ethers.js - [https://docs.ethers.io/v5/](https://docs.ethers.io/v5/)
- Docusaurus - [https://docusaurus.io/docs](https://docusaurus.io/docs)

#
