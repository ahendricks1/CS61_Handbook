# Array

A array is a ordered heterogenous collection of data, identified with an index. In Python, there is no built-in support, so we use lists.

# In Memory

In memory, an array looks like this:

![Image of an array in memory](images/array_memory.png)

The array is contiguous in memory, with each value placed in order in the next available memory address.

# Operations

An array supports the following operations:

* Access: Returns data according to its index, O(1), With the ability to use index to find a piece of data, as long as the index of the specific piece of data is known, accessing is in constant time.
* Search/Insertion/Deletion: Traversing an array to return a boolean value/Inserting data at a specific index in the array/Deleting data from the array, O(n), When searching, you must first traverse the list, but if you do not know what index the element is in, you must continue traversing the array. With insertion/deletion, once the element is found, you must then shift over all other elements, which results in O(n) time.

# Use Cases

An array is useful when you want to be able to keep your elements in order with indices.

It is not as good as a linked list if you want to insert/delete in constant time.

# Example

```
a = []
a.append("Dog")
a.append("Cat")
a.append("Giraffe"
print(a)
a.pop()
print(a)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
