# Project Name

OpenIoE - Implement bidirectional publish-subscribe behaviour 

## Student Info

- Name  : Priya Pappachan
- Email : priyapappachan010@gmail.com

### Project Abstract

OpenIoE is an open source project capable of retrieving and storing data from sensors with a web frontend to monitor and manage this sensor data. Currently, OpenIoE cannot act as a publisher and therefore cannot send control messages to sensors so as to change their settings. Therefore a user of OpenIoE cannot trigger a data collection from connected sensors immediately or in the future. Extending OpenIoE to support bi-directional pub-sub will enable it to send data collection requests to sensors. With this feature, OpenIoE will able to actuate sensors as necessary and thus act as a central platform from which a user can control their sensors as necessary.


### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#5416938311254016)

### [GSoC Project Proposal](https://docs.google.com/document/d/1XEJdqeMuNi51oeE49VmP2skFcLf9zB9SWev2GBFsvgw/edit?usp=sharing)

### [GitHub Organization Repo](https://github.com/scorelab/OpenIoE)

### [GitHub Personal Repo](https://github.com/priyapappachan/OpenIoE)

### [Commits during GSoC 2017](https://github.com/scorelab/OpenIoE/commits?author=priyapappachan)

### [Project Demo Video](https://drive.google.com/file/d/0B8TApYOf5vh0LW9UUVpYV2NrN0U/view)

### [Project Wiki](https://github.com/priyapappachan/OpenIoE/wiki/OpenIoE)

### Work Summary

The bidirectional publish-subscribe behaviour in OpenIoE is implemented using rest endpoint and Artemis message broker with the support of MQTT protocol. MQTT Topic Wildcards can be used for topic filters when subscribing to MQTT messages. These wildcards are useful if a client wants to receive messages for different topics with similar structure at once. The user can create a new subscription in OpenIoE to subscribe to topics of device sensors. The messages that are received on the subscribed topics are stored in Cassandra. The user can also create publications in OpenIoE to publish data to topics. The data can be published using HTTP or MQTT protocols. All data messages that are used for publish/subscribe are stored in Cassandra keyspace whereas sensor and device information are stored in MySQL database. An android application is developed to test the publish behavior by sending GPS sensor data from mobile device to other devices through OpenIoE. An MQTT client application can be used to subscribe to the required topics and to receive messages.


### What Covered

- Added bidirectional publish-subscribe behavior to OpenIoE
- Topic filter implementation for subscription to messages
- Developed an Android application to test OpenIoE with GPS sensor data
- Detailed documentation on installation, usage and concepts in OpenIoE

### What left

- Need to implement authentication for Publish Subscribe

### Reference

- [MQTT client](https://github.com/fusesource/mqtt-client) 
- [JHipster](https://jhipster.github.io/)
- [Artemis message broker](https://activemq.apache.org/artemis/)




