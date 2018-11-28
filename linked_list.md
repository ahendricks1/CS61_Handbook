# Linked List

A linked list is an unordered list of elements with the first item being referred to as the head, and the rest as the tail. Linked lists are not contiguous in memory, each node only knows the location of the next node. Two types of linked lists exist: Singly Linked, in which one node refers to the next, and Doubly linked, where each node refers to the previous and next node.

# In Memory

In memory, a linked list looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A linked list supports the following operations:

* Access/Search: Traverses through linked list till it reaches the value/Searches for the item in the list and returns a boolean, O(n), Since search starts at the head of the list, and linked lists are not contiguous in memory, therefore we may need to traverse through the whole list before reaching the requested element
* Insertion/Deletion: Inserts a new node into the list/Removes a node from the list, O(1), Like the search function, to insert/delete at a specific index we must first traverse the list O(n) until we reach the index, but then inserting the node requires only constant time steps to maneuver the nodes around so we don't lose the tail. With deletion the same process of searching must be taken, and deletion requires the reverse steps as insertion to maintain the linked list but still occurs in O(1) time.

# Use Cases

A  doubly linked list is useful when you aren't worried about being contiguous with your list and want O(1) insertion and deletion.

It is not as good an AVL tree if you wish to access/search through a large collection of data faster than O(n).

# Example

```
list = unordered_list()
list.append(5)
list.append(1)
list.remove(1)
list.search(1)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
