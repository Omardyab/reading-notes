#  Reading 29: Graphs


## Some common terminology used when working with Graphs:

    Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
    Edge - An edge is a connection between two nodes.
    Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
    Degree - The degree of a vertex is the number of edges connected to that vertex.


## Directed vs Undirected
Undirected Graphs
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

### Directed Graphs (Digraph)
A Directed Graph also called a Digraph is a graph where every edge is directed.

### Complete Graphs
A complete graph is when all nodes are connected to all other nodes.

### Connected
A connected graph is graph that has all of vertices/nodes have at least one edge.

### Disconnected
A disconnected graph is a graph where some vertices may not have edges.


## Acyclic Graph
An acyclic graph is a directed graph without cycles.

A cycle is when a node can be traversed through and potentially end up back at itself.

## Cyclic Graphs
A Cyclic graph is a graph that has cycles.

A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation
We represent graphs through:

Adjacency Matrix
Adjacency List