# Project Name
BellyDynamic: A scalable data structure to handle online and offline dynamic graph objects

## Student Info
Yasanka Sameera Horawalavithana

### Project Abstract
A social network evolves over time through the creation or deletion of ties among a set of actors.The volatile nature of social ties provides a strong platform to identify the dynamic network structure. This change of structural patterns can be well represented by the existence of dynamic graph objects Further, they can be enriched with the temporal information of social ties to define the recurrent subgraphs of interest. This would yield important insights about the correlation between patterns of ties in a social network. Major contribution of our study is the proposal and implementation of a scalable data structure to handle online and offline dynamic network objects. Hence, it can be used for large scale graph modeling, analysis and visualization purposes.

### [GSoC Project Page](https://summerofcode.withgoogle.com/projects/#6496645247139840)

### [GSoC Project Proposal](https://docs.google.com/document/d/1yMrNdxqeOQFSC3YMYAsw2HHhSG_gBjWZsRj5mP4f7a0/)

### [GitHub Organization Repo](https://github.com/scorelab/BellyDynamic)

### [GitHub Personal Repo](https://github.com/SamTube405/BellyDynamic)

### [Commits during GSoC 2017](https://github.com/scorelab/BellyDynamic/commits/master)

### [Project Wiki](https://github.com/SamTube405/BellyDynamic/wiki)

### Work Summary
BellyDynamic is wrapper on top of Snap: a popular graph processing framework, to capture multi-graphs. It handle dynamic updates to a graph object by maintaining all the states in a multi-graph format, annotated by node and edge level attributes. BellyDynamic was started from the scratch in my personal github repo, and consequently merged to organization github repo through PR and code reviews. The Wiki page (referred) would provide up-to-date information about the status of the project including 'How-to' articles via examples.

### What Covered
- Implemented basic module structure to handle multi-graphs
- Implemented basic classes to handle dynamic graphs in multi-graph format
- Implemented advanced classes to create graph objects from the scratch, and load graph datasets to an object
- Implemented general strategies to define user-level schemas
- Implemented container structure to store both node and edge attributes
- Implemented basic operations on top of graph attributes
- Implemented graph structural properties including centrality metrics
- Implemented automated continuous deployment strategies

### What left
- Need to implement advanced graph structural properties for dynamic/ multi graphs. Current setup only considers multi-graph as a collection of graphs. Graph structural properties that have been implemented so far would capture information related to static graphs.
- Need to implement a distributed data structure to handle fast dynamic graph updates.
- Need to implement an efficient index structure to query annotated graph information.
- Need to design a framework that supports cross-libraries (e.g. snap, networkx, igraph, Boost)

### Reference
[1] Leskovec, Jure, and Rok Sosič. "Snap: A general-purpose network analysis and graph-mining library." ACM Transactions on Intelligent Systems and Technology (TIST) 8.1 (2016): 1.
