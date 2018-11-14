# Dictionary

A dictionary is a heterogeneous, unordered structure consisting of key:value pairs, identified with curly braces {}.

# In Memory

In memory, a set looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A dictionary supports the following operations:

* .get(k): Returns the value associated with they key, O(1), since this structure is made up of key:value pairs, when given the key, we can return the value in constant time
* .values(): Returns the values of the dictionary, O(1), goes from one key to the next and returns each value
* .key(): Returns the keys of the dictionary, O(1), much like the .values(), just needs to traverse through the dictionary and return all keys

# Use Cases

A dictionary can be useful if you want to create a large list and have constant access time.

It is not as good as a list if you want to keep an ordered sequence of data, although allows for constant time no matter the length.

# Example

```
my_dict = {"Dog":"Bark", "Cat":"Meow", "Fish":"Blub"}
print(my_dict)
my_dict.values()
my_dict.keys()
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
