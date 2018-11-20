# Binary Search Tree

A binary search tree is an unbalanced tree data type that creates a map using keys with values in place.

# In Memory

In memory, a \[widget\] looks like this:

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
class Tree_node:
  
  def __init__(self, key, val, left = None, right = None, parent = None):
    self.key = key
    self.val = val
    self.left_child = left
    self.right_child = right
    self.parent = parent
    
   def has_left_child(self):
    return self.left_child
    
   def has_right_child(self):
    return self.right_child
    
   def is_root(self):
    return not self.parent
    
   def is_leaf(self):
    return not (self.right_child or self.left_child)
  
```

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
