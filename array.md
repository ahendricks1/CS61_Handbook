# Array

A array is a ordered heterogenous collection of data, identified with an index. In Python, there is no built-in support, so we use lists.

# In Memory

In memory, an array looks like this:

![Image of an array in memory](images/array_memory.png)

The array is contiguous in memory, with each value placed in order in the next available memory address.

# Operations

An array supports the following operations:

* Access: Returns data according to its index, O(1), With the ability to use an index to find a piece of data, as long as the index of the specific element is known, accessing is in constant time.
* Search/Insertion/Deletion: Traversing an array to return a boolean value/Inserting data at a specific index in the array/Deleting data from the array, O(n), When searching you must first traverse the list, but if you do not know what index the element is in, you must continue traversing the array. With insertion/deletion, once the element is found, you must then shift over all other elements, which results in O(n) time.

# Use Cases

An array is useful when you wish to keep a large collection of data and have O(1) access time.

It is not as good as a stack if you wish to insert and/or delete elements in a more efficient time.

# Example

```
a = []
a.append("Dog")
a.append("Cat")
a.append("Giraffe")
print(a)
a.pop()
print(a)
a.append("Dolphin")
a.remove("Cat")
print(a)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
