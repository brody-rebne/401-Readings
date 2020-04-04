## Trees

### What are Trees?

- Trees are a data structure built as a hierarchical graph of nodes
- In today's lecture+reading, we learned about a specific type called Binary Trees
- Binary Tree = max 2 child nodes per node
- Glossary:
  - Node: an item in the tree
  - Root: the node in the tree with no parent, the "top" node
  - Left Child: a child node which is positioned on the left
  - Right Child: take a wild guess
  - Edge: the link between a parent and child node
  - Leaf: a node with no children
  - Height: the number of edges ("levels") from the bottommost leaf to the root

### Sample Tree

![Sample Tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

### Binary Trees

- Binary trees are binary for easier traversal
- Traverse using Node.Left and Node.Right (like a doubly linked list)
- Nodes can be searched or used by pushing/enqueueing and popping/dequeueing them, placing them on the stack/queue to be peeked for information
- Binary trees are unstructured, so inserting and searching nodes will take O(n) complexity
- A Complete Binary Tree is one where every level is completely filled, except the bottom level
- A Full Binary Tree is one where every node either has 2 or 0 children
- A Perfect Binary Tree is one where every level is completely filled (effectively a Complete+Full Binary Tree)
