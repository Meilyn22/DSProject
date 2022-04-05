# Sorting Algorithms 

Sorting algorithms denote the ways to arrange data in a particular format. Sorting ensures that data searching is optimized to a high level and that the data is presented in a readable format. Let us look at the five different types of Sorting algorithms in Python:

Bubble Sort – This algorithm is based on comparison in which there is repeated swapping of adjacent elements if they are in an incorrect order.

Merge Sort – Based on the divide and conquer algorithm, Merge sort divides the Array into two halves, sorts them, and then combines them.

Insertion Sort – This sorting begins with comparing and sorting the first two elements. Then, the third element is compared with the two previously sorted elements and so on.

Shell Sort – It is a form of Insertion sort, but here, far away elements are sorted. A large sub-list of a given list is sorted, and the size of the list is progressively reduced until all the elements are sorted.

Selection Sort – This algorithm begins by finding the minimum value from a list of elements and puts it into a sorted list. The process is then repeated for each of the remaining elements in the list which is unsorted. The new element entering the sorted list is compared with its existing elements and placed at the correct position. The process goes on until all the elements are sorted.

# Searching Algorithms 

Searching algorithms help in checking and retrieving an element from different data structures. One type of searching algorithm applies the method of sequential search where the list is sequentially traversed, and every element is checked (linear search). In another type, the interval search, elements are searched for in sorted data structures (binary search). Let us look at some of the examples:

Linear Search – In this algorithm, each item is sequentially searched one by one.

Binary Search – The search interval is repeatedly divided in half. If the element to be searched is lower than the central component of the interval, the interval is narrowed to the lower half. Otherwise, it is narrowed to the upper half. The process is repeated until the value is found.

Graph Algorithms 
There are two methods of traversing graphs using their edges. These are:

Depth-first Traversal (DFS) – In this algorithm, a graph is traversed in a depthward motion. When any iteration faces a dead end, a stack is used to go to the next vertex and start a search. DFS is implemented in Python using the set data types.

Breadth-first Traversal (BFS) – In this algorithm, a graph is traversed in a breadthward motion. When any iteration faces a dead end, a queue is used to go to the next vertex and start a search. BFS is implemented in Python using the queue data structure.

# Algorithm Analysis 
A Priori Analysis – This represents a theoretical analysis of the algorithm before its implementation. An algorithm’s efficiency is measured by presuming that factors, such as processor speed, are constant and have no consequence on the algorithm.

A Posterior Analysis – This refers to the empirical analysis of the algorithm after its implementation. A programming language is used to implement the selected algorithm, followed by its execution on a computer. This analysis collects statistics, such as the time and space required for the algorithm to run.