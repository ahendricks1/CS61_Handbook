# Deque

A deque, also known as a, "double-ended queue" is an ordered collection of items much like a queue. The difference between the two is that a deque has no restriction on which end items are added.

# In Memory

In memory, a \[widget\] looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A deque supports the following operations:

* .addFront(item): adds a new item to the front of the deque, O(1), since a deque can act the same as a queue when appending a new item, we only need to know where the front of the list is to add a new item, thus giving us constant time.
* .addRear(item): adds a new item to the rear of the deque, O(1), just like .addFront(), addRear() just needs to look at the last item in the deque, and append.
* .removeFront(): removes the item at the front of the deque, O(1), the deque acts just like a queue in this scenario and can remove an item in constant time.
* .removeRear(): removes the last item of the deque, O(1), with no restriction on the hybrid linear structure, the last item can be popped off in constant time.

# Use Cases

A deque is useful when you want to create an ordered list of numbers, or you can use a deque to check a string to see if the sequence of items is the same both ways, passing a palindrome test.

It is not as good as queue if you wish to maintain an ordered collection of items that are dealt with according to who showed up first.

# Example

```
d = Deque()
d.addRear(4)
d.addRear("Dog")
d.addFront(3.4)
print(d)
d.removeRear()
d.removeFront()
print(d)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
