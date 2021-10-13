# Trees:
A tree is a nonlinear data structure, compared to arrays, linked lists, stacks and queues which are linear data structures. A tree can be empty with no nodes or a tree is a structure consisting of one node called the root and zero or one or more subtrees.

Today we will be talking about number of trees in data structure:
1. Binary Trees
2. Binary Search Trees
3. K-ary Trees

### Below are some common Terminology:

1. Node - A Tree node is a component which may contain it’s own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a **binary tree, k = 2**.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf.

### Traversing a tree:
There are two ways to traverse a tree:

1. Depth First: is where we prioritize going through the depth (height) of the tree first. And there are multiple ways to acomplish it (Stack) :
 * Pre-order: **ROOT ==> LEFT ==> RIGHT**.
 * In-order: **LEFT ==> ROOT ==> RIGHT**.
 * Post-orde: **LEFT ==> RIGHT ==>ROOT**. 
2. Breadth First: Breadth first traversal iterates through the tree by going through each level of the tree node-by-node (Queue).

## Binary Tree Vs K-ary Trees:
 Binary Trees restrict the number of children to two (Left and Right). Where as the K-ary tree Are able to have more than two child nodes In this case of tree we use **K** to refer to the maximum number of children that each Node is able to have.

 K-ary Trees it uses the same traversing techniques as a binary tree such as Breadth First Traversal.
 So to add a node to the K-ary trees we you can place the node where ever you want in your tree it dosent matter.

 ## BigO Trees:
 The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has n nodes, then in the worst case we will have to look at n items, hence the O(n) complexity.

 The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. For example, in the above tree, w is 4.

 ## Binary Search Tree:
 s a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

 ### Searching a Binary Search Tree:
 Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.

 ## BigO For BST:
 The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.
The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.


