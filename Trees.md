# Introduction to Trees
Trees like linked lists connect nodes through pointers. The tree is a non-linear data structure unlike with the following chracteristics :

1. The tree has a root node (this is marked by one node in the tree).
2. Every node except for the root node has one parent node.
3. The nodes can have varying number of children nodes.

The tree comprises of terminology that might be useful to your understanding of concepts:

* NODE:
    A node is an element in the tree.

* ROOT:
    A binary tree contains one root. The root has no parent and is the top most elelement..

* LEAF:
    We can describe the leaves of a tree as the nodes without children.

* HEIGHT:
    The Height is the generation of the respective nodes. The root has a height of 0, the children of the root node have a height of 1, the grandchildren of the root node have a height of 2 and so on

* PARENT:
     A parent is a node that connects to children nodes.

* CHILD:
    A child is a node connected from a parent node.

In this lesson we will only talk about the Binary tree in python.


## Binary Tree

The Binary tree is a data structure that is used for searching and data organization. Unlike many data structures in Python, the binary tree is non-linear.  A binary tree has up to two children for each node.

A binary tree node contains the following properties:

1. Data.
2. A pointer to the right node.
3. A pointer to the left node.

<p align="center">
    <img src= "https://byui-cse.github.io/cse212-course/lesson09/binary_tree.jpeg" alt= "Binary tree illustration">

    (*source*: Byui.edu)
</p>

## Inserting into a Binary Tree

