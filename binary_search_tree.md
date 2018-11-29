# Binary Search Tree

A binary search tree is an unbalanced tree data structure that creates a key/value map. BSTs start with a root node, and when new nodes are inserted their values are checked against the root nodes key and sorted accordingly with keys smaller than the root to the left, and larger to the right.

# In Memory

In memory, a binary search tree looks like this:

![Image of BST](binary_search_tree.jpg)

# Operations

A binary search tree supports the following operations:

* Access/Search: Returns the key/returns a boolean value after traversing the tree, O(logn), Accessing and/or binary searching typically cuts the issue of finding the correct node each time it is recursively called, resulting in O(logn) time. However, a standard BST can become unbalanced very quickly if all the keys are lesser/greater than the root node, accessing and searching can become dependent on the number of nodes in the tree.
* Insertion/Deletion: Inserts a new node into a BST/Deletes a node from a BST, O(logn), Much like the access/search, if the tree becomes too unbalanced, finding the next available spot to insert a node could take O(n). Likewise, traversing a tree to find the specific node to be deleted and then moving the other nodes accordingly could be O(n) complexity.

# Use Cases

A binary search tree is useful when searching/accessing a specific key, with the ability to use binary search to reduce the nodes needed to sift through by half every time (Best/average case) causing complexity to be O(logn)

It is not as good as an AVL tree because it is unable to consistently balance itself while new nodes are being inserted.

# Example

```
bst = BST(20)
bst.insert(5)
bst.insert(15)
bst.insert(46)
bst.remove(5)
bst.is_leaf(46)
```

[Previous](linked_list.md) [Next](avl_tree.md)

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
