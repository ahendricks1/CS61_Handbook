# Dictionary

A dictionary is a heterogeneous, unordered structure consisting of key:value pairs, identified with curly braces {}.

# In Memory

In memory, a set looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A dictionary supports the following operations:

* Get: Returns the value associated with they key, O(1), Since this structure is made up of key/value pairs, when given the key, we can return the value in constant time.
* Pop: Removes an element if the correct key is given, O(1), Much like get(), pop() is able to make use of the key/value pairs and remove the selected element in O(1) because of the corresponding key.
* Key: Returns the keys of the dictionary, O(1), Since keys() traverses each item one at a time, we are able to maintain a constant time of O(1).

# Use Cases

A dictionary can be useful if you want to create a large list and have constant access time.

It is not as good as a list if you want to keep an ordered sequence of data, although allows for constant time no matter the length.

# Example

```
my_dict = {"Dog":"Bark", "Cat":"Meow", "Fish":"Blub"}
print(my_dict)
my_dict.pop()
print(my_dict)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
