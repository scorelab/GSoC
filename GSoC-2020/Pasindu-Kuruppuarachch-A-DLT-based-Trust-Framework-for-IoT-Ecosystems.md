# A DLT-based Trust Framework for IoT Ecosystems

## Student Info

* Name - Pasindu Kuruppuarachchi
* Email - pasindualawaka91@gmail.com
* GitHub Profile - https://github.com/pasinduwalawaka
* Universtiy - Cork Institute of Technology


### Project Abstract
There are multiple stakeholders engaging in IIoT systems. For example in the energy and power
industry energy prosumers, consumers, regulators, traders, and community are few of the
stakeholders taking part. These stakeholders must trust each other to carry out business processes
smoothly and it will maximize the profit and efficiency of the entire industry. Furthermore,
centralization can course problems such as single point of failure, and bring extra friction to the
interoperability. As access control is one of the key methods enabling confidentiality and
integrity in IoT eco-systems measures should be taken to avoid a single point of failure and make
access control more trustworthy. This project will is an attempt to implement a decetralized access control mechanism
on Hyperledger Fabric. During this Google Summer of Code project we have focused on building a toolkit around the deployment
of this Access Control Model and the DLT network associated with it to help with the workflow of developers as well as end users.


### [GSoC Project Page](https://summerofcode.withgoogle.com/dashboard/project/4933314479128576/overview/)

### [GSoC Project Proposal](https://summerofcode.withgoogle.com/serve/6053633696727040/)

### GitHub Organization Repo
[HLF-Scaffold](https://github.com/leopardslab/hlf-scaffold) <br>
[D-IoT-A](https://github.com/leopardslab/d-iot-a)

### GitHub Personal Repo
[HLF-Scaffold](https://github.com/pasinduwalawaka/hlf-scaffold) <br>
[D-IoT-A](https://github.com/pasinduwalawaka/d-iot-a)


### [Commits during GSoC 2020]()
[HLF-Scaffold](https://github.com/leopardslab/hlf-scaffold/commits/master)
[D-IoT-A](https://github.com/leopardslab/d-iot-a/commits/master)


### Work Summary
Implemented the smart contracts that can handle a simple access granting/revokation process.
Implemented the test DLT network to deploy Access Control Depolyment. While developing we recogonize the potential deployment and development pipiline for a HLF-DLT based application. 
So that we mainly focused on building the necesory toolkit for a HLF based application where we implemented a tool tool is for setting up a Hyperledger Fabric network easily using minimal number of CLI commands.
This tool can be used to generate the necessory infrastructure and configurations for the Decentralized Access Control project. 


### What Covered
D-IoT-A
* Design a DLT consortium cosnsit of 4 Organizations (For testign purposes) which includes the configuration of the Crypto-Assets and Configtx. [`PR-1`](https://github.com/scorelab/Bassa/pull/918)
* Introduced the HLF-Scaffold to the developement and deployment pipeline. [`PR-2`](https://github.com/leopardslab/d-iot-a/pull/2) 
* Chaincode for testing the implemented DLT network. [`PR-4`](https://github.com/leopardslab/d-iot-a/pull/4)
* Chaincode for Access Control Handling. [`PR-5`](https://github.com/leopardslab/d-iot-a/pull/5)

HLF-Scaffold
* Desiging of the system architecture [`Wiki`](https://github.com/leopardslab/hlf-scaffold/wiki/Architecture)
* Implemented HLF and prerequists installation shell scripts [`PR-1`](https://github.com/leopardslab/hlf-scaffold/pull/1/files)
* Implemented the Crypto Config Generator [`PR-3`](https://github.com/leopardslab/hlf-scaffold/pull/3/files) |
[`PR-4`](https://github.com/leopardslab/hlf-scaffold/pull/4/files)
* Implemented the Configtx generation using Python YAML library [`PR-5`](https://github.com/leopardslab/hlf-scaffold/pull/5/files)
* Set of YAML assets needed in network generation [`PR-6`](https://github.com/leopardslab/hlf-scaffold/pull/6/files)
* Introduced the Ruamel YAML library for YAML file handling. It preserseved the comments and order of YMAL structure in Fabric configurations. [`PR-7`](https://github.com/leopardslab/hlf-scaffold/pull/7)


### What left
* Docker-Compose generation
* Functions for editing a consortium definition. 
* Chaincode for adding Access Policies
* Packaging
