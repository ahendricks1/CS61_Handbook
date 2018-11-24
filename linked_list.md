# Linked List

A linked list is an unordered list of items with the first item being referred to as the head, and the rest as the tail. Two types of linked lists exist: Singly Linked, in which one node refers to the next, and Doubly linked, where each node can refer to the previous and next node.

# In Memory

In memory, a \[widget\] looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A linked list supports the following operations:

* .search(item): searches for the item in the list and returns a boolean, O(n), since search starts at the head of the list, and linked lists are unordered, the requested item may be at any index, thus the search must go through the whole list.
* .insert(pos, item): returns the position of an item, O(n), like the search function, to insert at a specific position we must traverse until we reach that position, because it is an unordered list, it could take O(n) to reach that point.

# Use Cases

A  doubly linked list is useful when you want to be able to traverse both forward and back because each node knows what is in front and behind it.

It is not as good as list if you want to be able to access an item in constant time, and insert onto the end faster, although slower anywhere else.

# Example

```
'''
Node
'''
class Node:
    def __init__(self, initdata):
        self.data = initdata
        self.next = None
        self.last = None

    def get_data(self):
        return self.data
    
    def get_next(self):
        return self.next

    def set_data(self, newdata):
        self.data = newdata

    def set_next(self, newnext):
        self.next = newnext
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
