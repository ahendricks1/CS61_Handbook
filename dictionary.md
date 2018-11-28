# Dictionary

A dictionary is a heterogeneous, unordered structure consisting of unique key:value pairs, identified in Python with curly braces {}.

# In Memory

In memory, a dictionary looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A dictionary supports the following operations:

* Access/Search: Returns the value associated with they key/Returns a boolean value after indexing key, O(1), Since this structure is based around key:value pairs, we are able to access and/or search in constant time because we have use the key as an index value itself, thus we can access/search in constant time.
* Insertion/Deletion: Inserts a new key:value pair as long as there are no duplicates elsewhere in the dictionary/Removes a key:value pair from the dictionary, O(1), Since dictionaries are unordered, there is no need to find a specific spot for the newest key:value pair as long as it is unique. If we know the key that corresponds to the value we want to remove, we simply index to that key and remove the value in O(1) time.

# Use Cases

A dictionary can be useful if you want to create a large collection of data and have constant access time to a value using the unique key.

It is not as good as a list if you want to keep an ordered sequence of data, although allows for constant time no matter the length.

# Example

```
my_dict = {"Dog":"Bark", "Cat":"Meow", "Fish":"Blub"}
print(my_dict)
my_dict["Giraffe"] = "Giraffe Noise"
print(my_dict)
print(my_dict["Giraffe"])
```

[Previous](sets.md)    [Next](hash_table.md)

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
