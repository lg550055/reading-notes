# Stacks and Queues

> Stacks and Queues are elegant tools, abstract data types, for handling temporary data.

You can think of stacks and queues as arrays with restrictions.

When properly implemented, all operations (read, write and delete) on stacks and queues take O(1) time and O(1) space.

## Stacks
A stack has the following constraints:
- Data can be ***inserted only at the top*** of the stack
- Data can be ***deleted only from the top*** of the stack
- ***Only the last element*** of the stack ***can be read***

A stack only works Last in, First out (LIFO).

Stacks can be implemented with linked lists or regular lists:
- A properly configured linked list will restric the operations to meet the requirements of a stack
- With a regular list, we must be careful to only use 'pop', 'append', and read from the end of the list
- The code implementation is simpler with a regular list, but ensuring the restrictions reamin in place is harder
- Keep in mind that regular lists require contiguous memory blocks, while linked lists do not. This might be important when dealing with large stacks.

## Queues
A queue has the following constraints:
- Data can be ***inserted only at the end*** of the queue
- Data can be ***deleted only from the front*** of the queue
- ***Only the element at the front*** of the queue ***can be read***

A queue only works First in, First out (FIFO).

To operate in O(1) time and space, a queue can use a linked list but not a regular list.  However, the linked list must provide ready access to its *front* (first) and end (last) nodes.

---

### Resources

- [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

---

[Back to table of contents](../README.md)