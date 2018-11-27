# Binary Search Tree

A binary search tree is an unbalanced tree data structure that creates a key/value map. BSTs start with a root node, and when new nodes are inserted their values are checked against the root nodes value and sorted accordingly with values smaller than the root to the left, and larger to the right.

# In Memory

In memory, a binary search tree looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

A binary search tree supports the following operations:

* Access/Search: Returns the key/returns a boolean value after traversing the tree, O(n), A standard BST can become unbalanced very quickly if all the keys are lesser/greater than the root node, accessing and searching can become dependent on the number of nodes in the tree.
* Insertion/Deletion: Inserts a new node into a BST/Deletes a node from a BST, O(n), Much like the access/search, if the tree becomes too unbalanced, finding the next available spot to insert a node could take O(n). Likewise, traversing to the bottom of a tree to find a specific node and then moving the other nodes accordingly would be O(n) complexity.

# Use Cases

A binary search tree is useful when searching/accessing a specific key, with the ability to use binary search to reduce the nodes needed to sift through by half every time. (Best/average case)

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

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
