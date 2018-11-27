# Sets

A set is a heterogenous, unordered and mutable collection of data that does not allow duplicates and is identified in Python with curly braces {}.

# In Memory

In memory, a set looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A set supports the following operations:

* Add: Adds item to the set, O(1), since sets are implemented as hash functions you can directly access the end of list and add a unique value (key).
* Remove: Removes item from the set, O(1), same with add, you can directly access the piece of data you want removed from the set. If the item is not within the set, you will receive a KeyError message.

# Use Cases

A set is useful if you want an mutable collection of unique items that can be added and removed in O(1) time.

It is not as good as a dictionary if you want to maintain duplicates, but access them at different times depending on the situation. With the key:value pairs, you can assign specific keys to the same value to receive the data during a specific time.

# Example

```
my_set = {4.5, "Dog", False, 3}
print(my_set)
my_set.add(55)
print(my_set)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
