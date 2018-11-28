# AVL Trees (Balanced Binary Trees)

An AVL tree is a binary search tree, that self-balances with each new node inserted.

# In Memory

In memory, an AVL tree looks like this:

\[sketch or diagram\]

\[description of diagram\]

# Operations

An AVL tree supports the following operations:

* Access/Search: Searches for a specific key in the tree, O(log n), An AVL tree performs the same as a BST with its access and search functions. Although with an AVL constantly readjusting with each new node, we are able to maintain a complexity of O(log n) because it's limited to the trees height.
* Insertion/Deletion: Inserts/Deletes a node from the AVL tree, O(log n), Using rotations if necessary for each new node, a insertion/deletion function can maintain a complexity of O(log n) even in the worse cases. Since the trees height cannot exceed +1/-1 depth, when inserting or deleting, you must only rotate a level of 1.

# Use Cases

An AVL tree is useful when a large tree is constantly being accessed, and new nodes are then being placed in the tree.

It is not as good as a binary heap if you wish to be able to readjust the tree into a min/max priority queue.

# Example

```
'''
Rotation
'''
def rotate_left(self, rot_root):
  new_root = rot_root.right_child
  rot_root.right_child = new_root.left_child
  if new_root.left_child != None:
    new_rot.left_child.parent = rot_root
  new_root.parent = rot_root.parent
  if rot_root.is_root():
    self.root = new_root
  else:
    if rot_root.is_left_child():
      rot_root.parent.left_child = new_root
    else:
      rot_root.parent.right_child = new_root
  new_root.left_child = rot_root
  rot_root.parent = new_root
```

[Previous](binary_search_tree.md) [Next](stack.md)

(c) 2018 AUSTIN HENDRICKS. All rights reserved.
