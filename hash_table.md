# Hash Table

A hash table takes in a key and then uses a hash function, which is a unique algorithm to convert the key into an index, which then points at the original key which has now become a value.

In memory, a hash table looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A hash table supports the following operations:

* Search: Searches through the hash table for a specific index that corresponds to a value after it has gone through a hash function, O(n), When a hash maintains a perfect hash function, searching is capable in O(1) time, however with collisions it grows to O(n) because chaining can occur.
* Insertion/Deletion: Inserts a new key that is put through a hash function, which then becomes a value within the table/Searches through the table until it comes across the right index, and if chaining/open addressing was necessary finds the correct value to delete, O(n), Since hash tables all depends on the proper hash function to sort keys efficiently, with collisions occurring normally, the chance of complexity growing to O(n) is not uncommon.

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
