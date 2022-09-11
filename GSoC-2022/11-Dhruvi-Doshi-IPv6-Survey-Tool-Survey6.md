# Survey6

## Student Info
* Name: Dhruvi Doshi
* Email: drdoshi29@gmail.com
* GitHub: [dhruvi29](https://github.com/dhruvi29)
* Linkedin: [Dhruvi Doshi](https://www.linkedin.com/in/dhruvi-doshi-5007801a0/)
* Medium: [@dhruvidoshi](https://medium.com/@dhruvidoshi)

## Project Abstract
Ipv6 is the internet's future, and it necessitated a more scalable survey tool to comprehend how routing and DNS function. The purpose of this project is to create an IPv6 listener that will passively collect IPv6 traffic data as a passive data collection tool for cyber security research.
Survey6 is a geo-distributed grid application with C&C Server as its center and the probes as the packet collection application for intercepting IPv6 traffic on linux. 
![](https://user-images.githubusercontent.com/61967013/188655683-3ea1cac5-d18b-4d5b-9948-617963a0caf6.png)

## GSoC Project Page
* [GSoC 2022 with SCoRe Lab](https://summerofcode.withgoogle.com/programs/2022/projects/jlm7VZtC)

## GSoC Project Proposal
* [Survey6 project proposal](https://docs.google.com/document/d/1SFRqrwRQEgbbtDlJc0c8iOtR9-HyfF6REOoRmyy-sAM/edit?usp=sharing)

## GitHub Organization Repo
* [web-telescope/survey6](https://github.com/web-telescope/survey6)

## GitHub Personal Repo
* [dhruvi29/survey6](https://github.com/dhruvi29/survey6)

## Commits during GSoC 2022
* [web-telescope/survey6/commits/main?author=dhruvi29](https://github.com/web-telescope/survey6/commits/main?author=dhruvi29)

## Project Demo Video
* [Application Server Demo](https://drive.google.com/file/d/1kmxOZZXKXUTpBfkJcs1gcroiuIDU3tys/view?usp=sharing)
* [Application Probe Demo](https://drive.google.com/file/d/1fSBYXjHva7zfjUsIW2_bN7vebJO_SB8Q/view?usp=sharing)
* [Testing Demo](https://drive.google.com/file/d/1mlhD5XWk1s7ELlx36w6s4_0fUfeKQu8D/view?usp=sharing)

## Project Wiki
* [Survey6 README](https://github.com/web-telescope/survey6#readme)

## GSoC Blog(s)
* [GSOC’22 @SCoRe Lab](https://medium.com/scorelab/gsoc22-score-lab-3f02cdb91a22)
* [Capturing the packets…](https://medium.com/scorelab/gsoc-week-1-2-score-lab-22aa58610f37)
* [The Server: gRPC & Protobuf](https://medium.com/scorelab/the-server-grpc-protobuf-98a766b6b71b)
* [System Service & DB](https://medium.com/scorelab/system-service-db-683b6c652076)
* [Some implementation touches..](https://medium.com/scorelab/some-implementation-touches-ff7c8e844c1e)
* [Scripting Installation](https://medium.com/scorelab/scripting-installation-83b01933058d)
* [Packaging Overview](https://medium.com/scorelab/packaging-overview-74aaeead3655)
* [Debian packaging of a python project](https://medium.com/scorelab/debian-packaging-of-a-python-project-ca4dfac9ac98)
* [gRPC : tips, tricks and testing](https://medium.com/scorelab/grpc-tips-tricks-and-testing-1dbb89210cd3)

## Work Summary
This summer was a dawn of survey6. Architecture of the project was planned. Directory structure for `C&C Server` and `Probe` was decided (You can find them [here](https://github.com/dhruvi29/survey6/tree/main/C%26C%20Server#folder-structure) and [here](https://github.com/dhruvi29/survey6/tree/main/Probe#folder-structure)). A lot of implementation details were discussed, finalized and implemented, including [protobuf schema and services](https://github.com/web-telescope/survey6/issues), [database schema](https://github.com/dhruvi29/survey6/tree/main/C%26C%20Server/src/main/data#database-schema) and [packaging methodology](https://github.com/web-telescope/survey6/pull/16). During the GSOC period, I have also worked on creating a [test suite](https://github.com/dhruvi29/survey6/tree/main/C%26C%20Server/src/test) for the application and worked on the [documentation](https://github.com/web-telescope/survey6/pull/18).        


## What Covered
1. [PR1](https://github.com/web-telescope/survey6/pull/3)
    * Data Collection mechanism for probe
    * Save captured packets
    * Save metadata of catured packets
2. [PR2](https://github.com/web-telescope/survey6/pull/7)
    * System service for starting server 
    * gRPC server on port 32000
    * Adding Protobuf definitions
    * SQLite Connect
    * Implemented function to accept client connection rrquest & add client to the db
    * Implement client disconnection
3. [PR3](https://github.com/web-telescope/survey6/pull/11)
    * Setup script
    * aliasing system service
4. [PR4](https://github.com/web-telescope/survey6/pull/12)
    * Error handling
    * Logging
5. [PR5](https://github.com/web-telescope/survey6/pull/16)
    * wrote install, postinst script 
    * generated debian source package
    * tool bin file
    * packaging the tool
6. [PR6](https://github.com/web-telescope/survey6/pull/17)
    * Test Suite
7. [PR7](https://github.com/web-telescope/survey6/pull/18)| [PR 8](https://github.com/web-telescope/survey6/pull/21)
    * Usage and setup guide
    * Documentation 

## What left
* Heart beat check
* Sending packets from probe and recieving packets
* Hosting debian package
