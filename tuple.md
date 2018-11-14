# Tuples

A tuple is a heterogeneous, ordered immutable list, identified with parenthesis ().

# In Memory

In memory, a set looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A tuple supports the following operations:

* .append(item): Adds item to the tuple, O(1), since we know where the end of the list is, we can get there is a constant time
* .insert(i, item): inserts an item at the ith position, O(n), we must first find the ith position, and then shift all items after our inserted item to make room
* .pop()/.pop(i): Removes and returns the last item in the list, if you're looking for the ith item it's O(n) because you must traverse through the tuple till you reach the item, otherwise if you're popping the last item it's O(1)

# Use Cases

A tuple is useful if you want to create a list but with immutable items.

It is not as good as a list, because of its immutable items, unless you specifically want a sequence of data to remain unchangeable for its existence.

# Example

```
my_tuple = (4.5, "dog", 4, False)
print(my_tuple)
my_tuple.append(55)
print(my_tuple)
my_tuple.pop()
print(my_tuple)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
