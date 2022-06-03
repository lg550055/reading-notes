# Graphs
> A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

### Types of graphs
There are several wayt to classify graphs:

- Directed vs Undirected
  - Directed - each vertex is directed at another vertex, referenced as *next*
  - Undirected - edges are bi-directional

- Complete vs Connected vs Disconnected
  - Complete - all nodes are connected to all other nodes
  - Connected - each vertex has at least one edge
  - Disconnected - some vertices may not have edges

- Acyclic vs Cyclic
  - Acyclic - no cycles
  - Cyclic - has at least one cycle (a path of a positive length that starts and ends at the same vertex)

### Representation of graphs

- Adjacency Matrix - vertices = rows = columns; if there is an edge between two given vertices, then thre's a 1 at (r,c), otherwise 0.  In the case of a weighted graph, instead of a 1, the number represetns the weight.
- Adjacency List - list of vertices, each of which contains a list of its neighboor vertices

### Graph traversal
Traversing a graph is similar to traversing a tree.  However, since graphs can have cycles, we need to keep track of visited nodes.

- Breadth First - visit all the nodes that are closest to the root first
- Depth First - visit all the children of the root first.

### Examples of real-world use of graphs

- GPS and mapping
- Social networks
- Airline traffic

---

### Resources

- [Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)

---

[Back to table of contents](../README.md)
