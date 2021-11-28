# Introduction to Queues

Queues are fundamental to data structures in programming. A queue is a close “cousin” of the stack; it’s a collection of objects inserted and removed according to the FIFO (First-in, first-out) principle. Meaning that the entity put in the queue first leaves the line (queue) first, and the entity that enters the queue last gets removed at the end.

![FIFO Queue illustration. ](pictures\queue4.jpg)

The idea is that elements enter a queue through the back and are taken away from the front. An analogy for this is a line of individuals queuing to get on a carnival ride. Individuals waiting for such a ride enter at the rear of the line and get on the ride from the front of the line. To remember this concept, you can also use the acronym “FCFS,” which means first-come, first-served.

Another great example would be a car wash where cars queue up to get a wash. The vehicles stay in a line waiting for their turn. The first car to show up gets to wash first, while the last car remains until all other vehicles that came before it is gone. Now we can wash the last vehicle and close for the day when we have no vehicles left.

![Cars entering and leaving a car wash.](pictures\queue1.jpg)
(*Source*: Alamy.com)

Let’s have a look at one more example.

### The Movie Ticket Counter

![An illustration of a movie ticket counter.](pictures\queue2.png)
(*Source*: simplilearn.com)

Customers can only enter from the rear end and leave from the front in these ticket counters. All other paths are closed with the help of barricades. Furthermore, the person who enters the ticket line first will exit first and the last person will exit last.

![An illustration of a movie ticket counter.](pictures\queue3.png)
(*Source*: simplilearn.com)

Stores, theaters, reservation centers, and other similar services typically process customer requests according to the FIFO principle. In addition, many computing devices also use FIFO queues, such as a networked printer or a Web server responding to requests. Therefore, a queue would be a logical choice for a data structure to handle calls to a customer service center or a wait-list at a restaurant. 

## Operations and Structure Of Queues

Unlike arrays and linked list, items in a queue cannot be operated from their respective locations. They can only be operated from the rare or front position. Also the structure of a queue depends on the perspective of the programmer. 

![An illustration of a queue with back at the left.](pictures\queue5.png)
*An illustration of a queue with back at the left.*

(*source*: Wikipedia. com)

![An illustration of a queue with the back on the right.](pictures\queue6.png)
An illustration of a queue with the back on the right.

(*source*: Javapoint.com)

Queue P supports the following two fundamental methods:
1. `P.enqueue(i)`: Add element `i` to the back of `queue P`.
2. `P.dequeue()`: Remove and return the first element from `queue P`;
if the queue `is empty`, an error will occur.


Other methods supported are:

* `P.first()`: Return a reference to the element at the front of `queue P`, without removing it; an error occurs if the queue is empty.
* `P.is empty()`: Return True if queue P does not contain any elements.
* `len(P)`: Return the number of elements in `queue P`; in Python,
we implement this with the special method `len`.

```
NOTE: Remember that it's assumed that a newly created queue is empty.
```
The following table shows a series of queue operations and their
effects on an initially empty queue P of integers.

operation        | Return Value  | first <-- P --> last  |
---------        | ------------  | --------------------  |
P.enqueue(7)     |       -       |          [7]          |
P.enqueue(4)     |       -       |         [7, 4]        |
len(P)           |       2       |         [7, 4]        |
P.dequeue( )     |       7       |          [4]          |
P.is empty( )    |     False     |          [4]          |
P.dequeue( )     |       4       |          [ ]          |
P.is empty( )    |     True      |          [ ]          |
P.dequeue( )     |     “error”   |          [ ]          |
P.enqueue(7)     |       –       |          [7]          |
P.enqueue(9)     |       –       |         [7, 9]        |
P.first( )       |       7       |         [7, 9]        |
P.enqueue(4)     |       –       |         [7, 9, 4]     |
len(P)           |       3       |         [7, 9, 4]     |
P.dequeue( )     |       7       |         [9, 4]        |

(*Table source*: Data Structures and Algorithms in Python BY *Michael T. Goodrich, Roberto Tamassia, Michael H. Goldwasser*)