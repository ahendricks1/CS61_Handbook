# Sets

A set is a heterogenous, unordered and immutable list that does not allow duplicates and is identified with curly braces {}.

# In Memory

In memory, a set looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A set supports the following operations:

* .add(item): Adds item to the set, O(1), since sets are implemented as hash functions you can directly access the end of list and add
* .remove(item): Removes item from the set, O(1), same with remove, you can directly access the piece of data you want to remove

# Use Cases

An set is useful if you want an immutable list of unique items.

It is not as good as a dictionary if you're okay with duplicates within your structure, dictionaries using key-value pairs is an easier way to keep track of values.

# Example

```
my_set = {4.5, "Dog", False, 3}
print(my_set)
my_set.add(55)
print(my_set)
```

(c) 2018 YOUR NAME. All rights reserved.
