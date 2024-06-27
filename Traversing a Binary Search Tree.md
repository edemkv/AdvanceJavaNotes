Traversing a Binary Search Tree (BST) means visiting all the nodes in the tree in a specific order. There are three common ways to traverse a BST: In-Order, Pre-Order, and Post-Order. Let's break down each method in simple terms:

### 1. In-Order Traversal
In-Order traversal visits nodes in ascending order. For a BST, this means visiting nodes from the smallest to the largest value.

**Steps:**
1. **Visit the left subtree**: Move to the left child and repeat this process.
2. **Visit the root node**: Process the current node.
3. **Visit the right subtree**: Move to the right child and repeat this process.

**Example:**
For a BST with the structure:
```
    4
   / \
  2   6
 / \ / \
1  3 5  7
```
In-Order traversal would visit the nodes in this order: 1, 2, 3, 4, 5, 6, 7.

### 2. Pre-Order Traversal
Pre-Order traversal visits the root node before its children. This is useful for creating a copy of the tree.

**Steps:**
1. **Visit the root node**: Process the current node.
2. **Visit the left subtree**: Move to the left child and repeat this process.
3. **Visit the right subtree**: Move to the right child and repeat this process.

**Example:**
For the same BST:
```
    4
   / \
  2   6
 / \ / \
1  3 5  7
```
Pre-Order traversal would visit the nodes in this order: 4, 2, 1, 3, 6, 5, 7.

### 3. Post-Order Traversal
Post-Order traversal visits the root node after its children. This is useful for deleting nodes from the tree.

**Steps:**
1. **Visit the left subtree**: Move to the left child and repeat this process.
2. **Visit the right subtree**: Move to the right child and repeat this process.
3. **Visit the root node**: Process the current node.

**Example:**
For the same BST:
```
    4
   / \
  2   6
 / \ / \
1  3 5  7
```
Post-Order traversal would visit the nodes in this order: 1, 3, 2, 5, 7, 6, 4.

### Visualization
To help visualize these traversals, imagine walking around the tree and visiting nodes based on specific rules. For In-Order, you walk to the leftmost node first, then go up to visit the parent, and finally go to the right. For Pre-Order, you visit the current node first, then move left, then right. For Post-Order, you visit the children before the parent.

Understanding these traversal methods helps in various operations on a BST, such as searching, insertion, deletion, and balancing the tree.
