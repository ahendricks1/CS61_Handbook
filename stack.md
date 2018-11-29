# Stacks

A stack is an ordered collection of items where the addition and removal of items always takes place on the same end. The ordering is often referred to as LIFO, last-in first-out.

# In Memory

In memory, a stack looks like this:

![Image of a stack](images/stack.jpg)

# Operations

A stack supports the following operations:

* Push: Adds a new item to the top of the stack, O(1), With a stack being a linear structure, adding a new item is constant, much like stacking a plate of dishes.
* Pop: Removes the top item from the stack, O(1), Again with the LIFO ordering, removing an item is as simple as looking to the top of the stack for the item that will be removed.
* Peek: Returns the value on the top of the stack without removing it, O(1), Peek acts almost the same as pop in the sense that it follows all of the same steps besides removing the item from the stack, it is put back on the top of the stack once it is done being 'peeked' at, which results in O(1) time.

# Use Cases

A stack is useful if you want an ordered list with a constant push/pop time complexity.

It is not as good as a queue if you want to access anything other than the data at the top of the stack. With a queue you are able to keep the data moving and reduces complexity because it follows FIFO ordering.

# Example

```
s = Stack()
s.push("dog")
s.push(4)
s.push(5.6)
print(s)
s.pop()
print(s)
s.peek()
```

[Previous](hash_table.md) [Next](array.md)

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
