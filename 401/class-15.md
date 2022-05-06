# Trees
This document gives an overview of Binary Trees, Binary Search Trees, and K-ary Trees.

### Common Terminology
- Node - A Tree node is a component which may contain its own values, and references to other nodes
- Root - The root is the node at the beginning of the tree
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf

### Traversals
There are two categories of tree traversals:

- **Depth First (DFS)** -recursively go through the depth of the tree first, in one of three ways for a binary tree:
  - ***Pre-order***: `root >> left >> right`
  - ***In-order***: `left >> root >> right`
  - ***Post-order***: `left >> right >> root`
- **Breadth First (BFS)** -go through each level of the tree node-by-node (commonly left to right with the use of a queue)

#### Binary Tree Vs K-ary Trees
For a K-ary tree (whose nodes allow more than 2 children).

### Adding a node
Unless there are specific rules for placing nodes, it is advantageous to fill all child spots top down, which maximizes balance.  To do so, use BFS to find the first node without all its children filled.

### Big O
- Unless there are specific organization rules for the tree, search and insertion have O(n) time complexity.
- BFS insertion has O(w) -> ~ O(n/2) -> O(n) space complexity.


### Binary Search Trees (BST)
In a BST, nodes with smaller values than the parent are placed to its left, and larger values to its right.  This makes searching fast, because the maximum number of search steps equals the height of the tree, which is logN.

BST are an efficient data structure.

---

### Resources

- [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

---

[Back to table of contents](../README.md)