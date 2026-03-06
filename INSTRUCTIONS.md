# Submission Instructions

## Week 1

1. Pick a social network among the ones proposed on `luiss.learn`.
2. Implement it in Python.
3. Draw the graph.
4. Compute the following quantities and comment on them:
   - number of nodes
   - number of edges
   - average degree
   - density

Be careful whether the network you picked is directed or undirected.

## Week 2

While considering the largest component of your network:

1. Design:
   - a function that computes the clustering coefficient for every node
   - another function that computes the average clustering coefficient
2. Compare your results to the built-in functions for average clustering and transitivity.

## Week 3

1. Compute the cumulative distribution of clustering.
2. For every node, define the average clustering of its neighbors and compute its cumulative distribution.
3. Compare the two distributions.

## Weeks 5-6-7

### Week 5

1. Depending on what seems most relevant in your graph, pick two of the following local notions:
   - decay centrality
   - betweenness centrality
   - closeness centrality
   - PageRank
   - any other notion you invent
2. Identify the most central nodes.

### Week 6

Treat your graph as undirected and unweighted. Delete loops and work on the resulting largest connected component.

Implement two of the following three techniques for community detection:

- bridge removal (pick the partition with the highest modularity)
- modularity optimization
- label propagation

In this case, you are allowed to use built-in functions from NetworkX.

Discuss which method you think is the best and why.

Provide a visualization for the partition you decided is the best using [Gephi Lite](https://gephi.org/gephi-lite/).

### Week 7

Treat your graph as undirected and unweighted, delete loops, and work on the resulting largest connected component.

1. Create a function computing CN and one of the following topological indices:
   - JI
   - PA
   - AA
   - RA
2. Your function should return a pandas DataFrame where:
   - each row is a missing link
   - each column is an index
3. You are allowed to use built-in functions from NetworkX to compute the individual indices.
4. Create a third score by adding a column with the sum of the two indices.

Note: the arithmetic mean should be computed after rescaling each column between 0 and 1.

For each of the three scores, identify as missing links the node pairs yielding the largest 5 or 10 values. Briefly comment on the results.

## Weeks 9-10

### Week 9

Depending on what seems most appropriate for your graph, pick one of the following random graph models:

- Erdős-Rényi
- uniform attachment
- preferential attachment
- a variant of one of the previous models invented by you (best option)

Using this method, choose the correct parameters to create a graph with:

- the correct number of nodes
- the correct average degree

Compare at least one other characteristic, such as:

- average clustering
- degree distribution
- transitivity
- average distance from one node
- diameter
- a centrality distribution

Comment on the results.

### Week 10

1. Depending on what seems most relevant in your graph, write the code for one of the following alternative models:
   - synchronous threshold model
   - asynchronous threshold model (random order)
   - synchronous fractional threshold model
   - fractional threshold model (random order)
   - independent cascade model
   - Bass contagion model
   - SIS model
   - a variant that seems pertinent for your graph
2. Investigate different outbreak scenarios in your graph, considering:
   - different outbreak sizes
   - different origins
   - different parameters
