# Trees data structure is used to decrease the time complexity of data search operations:

## Common Terminology

- Node - A Tree node is a component which may contain its own values, and references to other nodes
- Root - The root is the node at the beginning of the tree
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf 

## Trees:

### Binary Trees

Binary trees are a type of tree where each node can have at most two children. They consist of nodes that have a left child and a right child, forming a hierarchical structure. Binary trees are used to represent various data structures and algorithms, such as binary search trees and binary heaps. They are versatile and can be efficiently traversed and searched.

### Binary Search Trees (BSTs)

Binary search trees are a specific type of binary tree that follows a specific ordering property. In a BST, the left child of a node contains a value smaller than the parent, and the right child contains a value greater than the parent. This property enables efficient searching, insertion, and deletion operations. BSTs are commonly used for tasks such as maintaining a sorted collection of data and implementing efficient search algorithms.

### K-ary Trees

K-ary trees are trees where each node can have up to K children. They generalize binary trees, where K is equal to 2. K-ary trees are useful when representing hierarchical relationships with more than two child nodes per parent. They find applications in areas such as file systems, databases, and organizational structures. K-ary trees allow for more flexible and complex hierarchies.

Each type of tree serves different purposes and has unique characteristics. Binary trees provide a simple hierarchical structure, binary search trees offer efficient searching and sorting, and K-ary trees accommodate more complex hierarchies. Understanding these tree types can help in solving various problems and designing efficient algorithms. The tree method uses dequeue and enqueue to search for data.

## Big O for each tree

### Binary Trees

- Searching: O(n) - In the worst case, you may need to visit every node to find the desired element.
- Insertion: O(1) - If you have a reference to the parent node, you can insert a new node in constant time.
- Deletion: O(1) - Similar to insertion, if you have a reference to the parent node and the node to delete, you can remove it in constant time.
- Traversal (in-order, pre-order, post-order): O(n) - You need to visit every node once to traverse the entire tree.

### Binary Search Trees (BSTs)

- Searching: O(log n) - In a balanced BST, the time complexity is logarithmic because you eliminate half of the tree at each comparison.
- Insertion: O(log n) - Similar to searching, you need to find the correct position in the tree, resulting in a logarithmic time complexity.
- Deletion: O(log n) - Deleting a node involves searching for the node to delete and adjusting the tree, resulting in logarithmic time complexity.
- Traversal (in-order, pre-order, post-order): O(n) - Regardless of the tree's balance, you need to visit every node once for traversal.

### K-ary Trees

- Searching: O(n) - In the worst case, you may need to visit every node to find the desired element.
- Insertion: O(1) - If you have a reference to the parent node, you can insert a new child node in constant time.
- Deletion: O(n) - Deleting a node involves searching for the node to delete and adjusting the tree, which may require visiting multiple nodes.
- Traversal (pre-order, post-order): O(n) - You need to visit every node once to traverse the entire tree. The time complexity is linear with respect to the number of nodes.
