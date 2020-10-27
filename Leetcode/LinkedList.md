# Linked List

### [426. Convert Binary Search Tree to Sorted Doubly Linked List](https://leetcode.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list/)


**Key: tree to doubly linked list**

1. Define two functions, `leftmost` and `rightmost` to find the leftest child and rightest child.
2. Define a helper function:
   
   2.1 If `node == None : return None`
   
   2.2 `self.helper(node.left)`
   
   2.3 node.left = rightmost child of node.left, and node becomes right child of rightmost child of node.left

   2.4 `self.helper(node.right)`

   2.5 node.right = leftmost child of node.right, and node becomes left child of leftmost child of node.right