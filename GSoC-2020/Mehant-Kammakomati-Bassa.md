# Integrate a cluster monitoring and alerting system using Prometheus for the Bassa kubernetes cluster and write client libraries for better usage of Bassa API server.

## Student Info

  * Name - Mehant Kammakomati
  * Email - kmehant@gmail.com / kmehant@scorelab.org / 411843@student.nitandhra.ac.in
  * University - National Institute of Technology, Andhra Pradesh
  * GitHub profile - https://github.com/kmehant
  * LinkedIn profile - https://www.linkedin.com/in/mehant-kammakomati-1a0b41170/
  * Medium - https://medium.com/@kmehant
  * Twitter - https://twitter.com/mehant1

### Project Abstract
Bassa has got container based on-premise deployment infrastructure using Docker and Kubernetes orchestration tool. As part of the infra, there is a potential need for a monitoring and alerting server for the cluster.

Bassa has a dedicated API server that serves the purpose of an automated download queue. Writing efficient client libraries would surely be a great use for other developers to easily integrate the automated download queue into their projects.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6437527856087040)

### [GSoC Project Proposal](https://docs.google.com/document/d/1AdwlHBf5e72-i35UAMCDPVUFf7s1czS2sET6nRGXWHI/edit)

### GitHub Organization Repo
[Bassa](https://github.com/scorelab/bassa) 

[Bassa Client Libraries](https://github.com/scorelab/bassa-client-libraries)

### GitHub Personal Repo
[Bassa](https://github.com/kmehant/bassa) 

[Bassa Client Libraries](https://github.com/kmehant/bassaClient)

### Commits during GSoC 2020
[Bassa](https://github.com/scorelab/bassa/pulls?q=is%3Apr+author%3Akmehant+) 

[Bassa Client Libraries](https://github.com/scorelab/bassa-client-libraries/pulls?q=is%3Apr+author%3Akmehant+)

### Project Demo Video

### [GSoC Blog](https://medium.com/@kmehant/gsoc-2020-medium-posts-at-one-place-85847bc303e)

### Work Summary
Fixed some potential Bassa server bugs on multi-threading and start operation.
Written K8s scripts for monitoring and alerting Bassa cluster using Prometheus and Grafana dashboards. Written client libraries for Bassa automated download queue in Python and Golang with timeouts, retry and rate-limiting features.

### What Covered
* Fixed type errors and added logging to MySQL operations. Fixed multi-threading issue, compression feature and other related bugs. [`PR-1`](https://github.com/scorelab/Bassa/pull/918)
* Fixed Travis pipeline. [`PR-1`](https://github.com/scorelab/Bassa/pull/921)
* K8s scripts for monitoring and alerting system using Prometheus and Grafana dashboards. [`PR-1`](https://github.com/scorelab/Bassa/pull/925)
* Get Bassa Backend URL from env, made a workaround for now. [`PR-1`](https://github.com/scorelab/Bassa/pull/927)
* Written Python Client Library with retry, timeout and rate-limiting features. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/1) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/3)
* Added unittests, documentation, run bassa for tests and GitHub actions pipeline for tests and push to PyPi. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/4) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/5) | [`PR-3`](https://github.com/scorelab/bassa-client-libraries/pull/9) | [`PR-4`](https://github.com/scorelab/bassa-client-libraries/pull/11) | [`PR-5`](https://github.com/scorelab/bassa-client-libraries/pull/13) | [`PR-6`](https://github.com/scorelab/bassa-client-libraries/pull/16) | [`PR-7`](https://github.com/scorelab/bassa-client-libraries/pull/20) | [`PR-8`](https://github.com/scorelab/bassa-client-libraries/pull/22)
* Add Golang Client library with timeout, retry and rate-limiting features. [`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/25)
* Add mandatory artifacts and services for the new GitHub repository - Bassa Client Libraries. 
[`PR-1`](https://github.com/scorelab/bassa-client-libraries/pull/6) | [`PR-2`](https://github.com/scorelab/bassa-client-libraries/pull/17) | [`PR-3`](https://github.com/scorelab/bassa-client-libraries/pull/18) | [`PR-4`](https://github.com/scorelab/bassa-client-libraries/pull/19) | [`PR-5`](https://github.com/scorelab/bassa-client-libraries/pull/21)

### What left
* Make Bassa v1.0 deployment - *not strictly part of the proposal*
* Review security layers for Bassa server and add any needed patches - *not part of the proposal*

### Reference
[Project Log Book](https://docs.google.com/document/d/1IdRkZhgs-HlXeYaRERVtWMzvFRyUDxmS6n-0sCCIPi4/edit?usp=sharing)