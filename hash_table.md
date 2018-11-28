# Hash Table

A hash table, much like a dictionary or BST, uses a map of key/value pairs to keep a collection so it may be searched in O(1) time (best/average case). It uses a unique algorithm, a hash function, to give an item a specific integer that is easily accessible.

# In Memory

In memory, a hash table looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A hash table supports the following operations:

* Search: Searches through the hash table for a specific integer that corresponds to an item after it has gone through a hash function, O(n), When a hash maintains a perfect hash function, searching is capable in O(1) time, however with collisions it grows to O(n) because chaining occurs.
* Insertion/Deletion: Inserts a new item that is put through a hash function, which then becomes an integer within the table/Searches through the table until it comes across the right integer, and if chaining/open addressing was necessary finds the correct item to delete, O(n), Since hash tables all depends on the proper hash function to sort items efficiently, with collisions occurring normally, the chance of complexity growing to O(n) is not uncommon.

# Use Cases

A hash table is useful when you wish to search for an item in O(1) time if you're able to maintain the best/average case. If collision is not an issue, all that is necessary is the correct hash value to find your item.

It is not as good as an AVL tree if you wish to maintain constant big-o complexity at all times. With collisions being a common occurrence, hash tables can become slow very quickly.

# Example

```
sample code showing creation, and exercising all of the operations
or
a program that doesn't use the structure, and then a version that does
```

[Previous](dictionary.md) [Next](stack.md)

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
