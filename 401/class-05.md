# Linked Lists

## Definition
A linked list is data structure that contains nodes that point to the next or previous node in the list:
- Each node contains information in addition to it's pointer(s)
- The first node is called the Head
- The reference to the next node is labled Next (and Previous when previous is present)

There are two types of linked lists:
- *Singly* - each node has a single reference that points to the next node in the list
- - *Doubly* - each node has two references, one pointing to the previous node and one to the next

## Traversal
Unlike regular lists, where one can traverse using loops, to traverse linked lists one must use the Next (or Previous) property.

A while loop is an efficient way to traverse.  The loop stops when we reach the last node, which has an empty next property.

Traversal has a time complexity of O(N), because in the worse case we have to go through the whole list.  Space complexity is O(1), because there's no addition need for space beyound the input.

## Adding Nodes

#### Adding a Head Node
Done in time O(1), add a new Node pointing to the Head and reassign Head to the new node.

#### Adding an intermediate Node
Done in time O(N), because we may have to traverse through the whole list, reassign the Next property of the node after which we are adding the new node and assign that value to the pointer of the new node.  In other words, point the previous node to the new node, and point the new node to the node to which the previous node was pointing before the insertion.  (If a Doubly, then do the correspoinding assignments with the Previous property of the new node and its neighboor nodes.)

## Keep in mind

- Implement a class Node that requires a value property
- A Linked list is linear data structure, which requires sequential traversing
- Linked lists do not reside in contiguous memory blocks- this has:
  - Advantages:
      - grow / shrink dynamically, which is helpful if the size of the list is variable
      - inserting and deleting is simple (just reassign pointers)
  - Disadvantages:
      - slow to traverse / search / slice
- There is a Circular linked list (that naturally can not be traversed until Next is empty)

---

## Algorith Efficiency - Big O
Introduced in previous notes, Big O describes the worst-case efficiency of an algorithm in terms of:
- Time - order of growth in number of operations vs input size
- Space - order of growth in amount of memory resources vs input size

*input size = n, where n is the size of the parameter values of the algorithm*

Memory resources are driven by working space, which includes stack space for recursive calls.  Working space is the memory resources needed to create variables and references.

![Order of growth table](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/OrdersOfGrowth.png)
Source: CodeFellows

#### Best, Average and Worst case
Even through Big O describe the wrost case, it is important to understand the average (and best) case.  For example, if our dataset has very thin tails, then choosing an algorithm with better average case performance would be to our advantage; even if its worst case performance is suboptimal.

- Big O - worst case
- Big Theta - average case
- Big Omega - best case

![Efficiency of code table](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/EfficiencyNotations.png)
Source: CodeFellows

---

### Resources

- [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
- [What’s a Linked List -1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
- [What’s a Linked List -2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)
- [Big O Algorith Efficiency](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)

---

[Back to table of contents](../README.md)