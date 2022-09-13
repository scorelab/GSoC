# Project Name
KubeBot

# Project Abstract
Kubernetes is a great tool for container orchestration, running Kubernetes in your production environment is getting traction in the Cloud industry. With growing DevOps tools, it is now a tedious and time-consuming task SREs and developers to continuously monitor their remote applications running inside a multicluster Kubernetes environment. Though there are some great tools using which we can monitor Kubernetes tools there is a need for easy deployment setup and an alerting tool that people can use to get alerts when something goes wrong inside their application running in a Kubernetes environment. It is often time-consuming to figure out the root cause of such issues, and most importantly not all alerts and issues are important and do not need human interaction. This brings us to address the problem of out of box metrics, traces, events and logs collection for applications running inside Kubernetes, reporting all the collected data on a single dashboard and push notifications to users for critical ones. The collected metrics, traces, events and logs will help to debug the application running inside Kubernetes faster and effectively.

## [GSoC Project Page](https://summerofcode.withgoogle.com/programs/2022/projects/CrF9bzaI)

## [GSoC Project Proposal](https://github.com/leopardslab/kubebot/blob/main/Kubebot_GSoC_Proposal.pdf)

## [GitHub Organization Repo](https://github.com/leopardslab/kubebot)

## [GitHub Personal Repo](https://github.com/priyanshuraj400/kubebot---GSoC-2022)

## Commits during GSoC 2022

| PR Link | Status | Issues |
| --- | --- | --- |
| [#6](https://github.com/leopardslab/kubebot/pull/6) | Merged ✅ | [#4](https://github.com/leopardslab/kubebot/issues/4) [#3](https://github.com/leopardslab/kubebot/issues/3) |
| [#10](https://github.com/leopardslab/kubebot/pull/10) | Merged ✅ | [#16](https://github.com/leopardslab/kubebot/issues/16) [#12](https://github.com/leopardslab/kubebot/issues/12) |
| [#11](https://github.com/leopardslab/kubebot/pull/11) | Merged ✅ | [#15](https://github.com/leopardslab/kubebot/issues/15) [#14](https://github.com/leopardslab/kubebot/issues/14) |
| [#19](https://github.com/leopardslab/kubebot/pull/19) | Merged ✅ | [#16](https://github.com/leopardslab/kubebot/issues/16) [#15](https://github.com/leopardslab/kubebot/issues/15) [#13](https://github.com/leopardslab/kubebot/issues/13) [#8](https://github.com/leopardslab/kubebot/issues/8) [#7](https://github.com/leopardslab/kubebot/issues/7) [#17](https://github.com/leopardslab/kubebot/issues/17) [#18](https://github.com/leopardslab/kubebot/issues/18) |
| [#9](https://github.com/leopardslab/kubebot/pull/9) | Merged ✅ | [#13](https://github.com/leopardslab/kubebot/issues/13) [#8](https://github.com/leopardslab/kubebot/issues/8) [#7](https://github.com/leopardslab/kubebot/issues/7) |
| [#27](https://github.com/leopardslab/kubebot/pull/27) | Merged ✅ | [#21](https://github.com/leopardslab/kubebot/issues/21) [#20](https://github.com/leopardslab/kubebot/issues/20) |
| [#28](https://github.com/leopardslab/kubebot/pull/28) | Merged ✅ | [#26](https://github.com/leopardslab/kubebot/issues/26) [#22](https://github.com/leopardslab/kubebot/issues/22) |
| [#29](https://github.com/leopardslab/kubebot/pull/29) | Merged ✅ | [#25](https://github.com/leopardslab/kubebot/issues/25) [#24](https://github.com/leopardslab/kubebot/issues/24) [#23](https://github.com/leopardslab/kubebot/issues/23) |


## [Project Demo Video](https://drive.google.com/drive/folders/1YAop5fDTnFnsKy6Oj4M6hsUSC49eIW1a?usp=sharing)

## [Project Wiki](https://github.com/leopardslab/kubebot)

## [GSoC Blog](https://medium.com/@priyanshuraj400)

# Work Summary

Kubernetes is a great tool for container orchestration, running Kubernetes in your production environment is getting traction in the Cloud industry. With growing DevOps tools, it is now a tedious and time-consuming task SREs and developers to continuously monitor their remote applications running inside a multicluster Kubernetes environment. Though there are some great tools using which we can monitor Kubernetes tools there is a need for easy deployment setup and an alerting tool that people can use to get alerts when something goes wrong inside their application running in a Kubernetes environment. It is often time-consuming to figure out the root cause of such issues, and most importantly not all alerts and issues are important and do not need human interaction.

KubeBot is a smart tool that pulls out of box metrics, traces, events and logs collection for applications running inside Kubernetes and reports all the collected data on a single dashboard and push notifications to users for critical ones. The collected metrics, traces, events and logs will help to debug the application running inside Kubernetes faster and effectively. A main feature of KubeBot is that after collecting traces, it does a root-cause analysis and sends alerts to the user regarding fixing the issue occuring in the cluster.


# What Covered

1. Helm chart to install KubeBot
2. Chart includes auto-configured montioring stack, i.e. Prometheus and Grafana.
3. Prometheus capable of pulling metrics and export to Grafana.
4. Auto installation of OpenTelemetry Collector with same helm chart.
5. End-to-End unit testing to validate monitoring stack deployment.
6. Added a log collector agent to ingest all the application logs > [filebeat](https://www.elastic.co/guide/en/beats/filebeat/current/filebeat-installation-configuration.html).
7. Developed a codec to compress the collected log output in the OTLP packet.
8. Developed an exporter to export the compressed OTLP packets.
9. Built exporter on gRPC.
10. Tested the resulting log collection agent by running it as a Deamonset.
11. End-to-End unit testing of entire program.


# What left

- Storing the logs from OTEL in a database and creating an ML model.
