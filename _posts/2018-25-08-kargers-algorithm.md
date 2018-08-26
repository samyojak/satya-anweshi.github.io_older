---
layout: post
title: "Karger's Algorithm"
date: 2018-08-25
tags: [graph, algorithm, clustering]
comments: true

---

## Graph
A set of vertices V along with set of edges E connecting these vertices in is called graph and denoted as $$ G=(V,E) $$. Example include a social network where each individual can be considered as vertex and any kind of relationship between two individuals can be considered as an edge. Another example is road network connecting different cities. Graph can be undirected where direction of an edge does not matter, it can be directed, when edges have direction, and direction has meaning associated. Below is an example of graph, each of vertex represents a city and edge represents flight connectivity.
[!Flights]({{site.baseurl}}/assets/img/my-image.jpg)

## Minimum Cut 
A cut in an undirected graph $$ G=(V,E) $$ is a partition of the vertices V into two non-empty, disjoint sets $$ S \bigcup T = V $$. Cutset of cut consits of the only edges connecting the vertcies in S to vertices in T. Number of edges in cutset is called size of cut. The cut with minimum size is called minimum cut.

Each vertex can be in either in set S or set T, hence there are $$ 2^V $$ cuts. Out of these two sets are empty, also interchanging S and T does not make any difference. Hence total valid cuts are $$ 2^{V-1} -1 $$. We need to find cut with minimum size among all cuts.


