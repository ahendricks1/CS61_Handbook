# Queues

A queue is a linear, ordered collection of items that follow the FIFO (first-in first-out) principle.

# In Memory

In memory, a \[widget\] looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A queue supports the following operations:

* .enqueue(item): adds a new item to the rear of the queue, O(1), since queues follow the FIFO rule, queueing is a constant complexity since it only needs to which item was added last to the queue.
* .dequeue(): removes the front item from the queue, O(1), again following the FIFO rule, the queue only needs to look at the 'front' of the line to see which item will be removed, no need to search through the queue.

# Use Cases

A queue is useful when order and position must be known. If you've got a room of students who must each print a paper, having a queue will allow the printer to know who pushed the print button first/last, and print those papers accordingly.

It is not as good as deque because it does not allow items to be added to the front if priority for a particular item is enacted.

# Example

```
q = Queue()
q.enqueue(4)
q.enqueue("Dog")
q.enqueue(3.5)
print(q)
q.dequeue
print(q)
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
