# London Gang Network Analysis

A tidy approach network analysis on the London-based inner-city street gang data from 2005 to 2009, concerning black people, operating from a social housing estate that have co-offended together. Data is available on [UCINET Software website](https://sites.google.com/site/ucinetsoftware/datasets/covert-networks/londongang) and comes from anonymised police arrest and conviction data for **all confirmed** members of the gang.

The network is **undirected** and it has 54 nodes representing the monitored people having the following attributes:

- ```Person```, representing the person’s **identifier**,
- ```Age```, representing the **age** of such person,
- ```Birthplace```, representing the **birthplace** of such person (1 for West Africa, 2 for Caribbean, 3 for United Kingdom, and 4 for East Africa),
- ```Residence```, representing the fact that the person was **resident**,
- ```Arrests```, representing the **number of arrests** of such person,
- ```Convictions```, representing the **number of convictions** of such person,
- ```Prison```, representing the fact that such person had already been **arrested**,
- ```Music```, representing the fact that such person **listened to music**,
- ```Ranking```, representing a **ranking** of such person.

The ties of such network are given as a **weighted adjacency matrix**, i.e. a 54×54 (weighted) matrix, where the weights are:

- 1, representing the fact that the connected people have **hanged-out**,
- 2, representing the fact that the connected people have **co-offended together**,
- 3, representing the facts that the connected people have **co-offended together** and that they have **committed serious crimes**,
- 4, representing the facts that the connected people have **co-offended together**, **committed serious crimes** and that there is a **kin relationship** (i.e. a family relationship) in-between nodes.

# Information about the repository
In this repository you will find:

- the used data,
- the R markdown of the analysis,
- the html rendering of such analysis.

# License
© Stan I. Eduard, Computer Science M.Sc. Student at the Università degli Studi di Udine.

Licensed under the [MIT License](LICENSE.md).
