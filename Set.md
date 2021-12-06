# Introduction to sets in Python
In this lesson, we are going to learn about sets in the Python programing language.

A set is a collection of unordered elements that are unique. In Python, sets are extraordinary because they have no duplicate values or items, so we can utilize them to eliminate duplicate elements from lists and tuples effectively. In addition, the elements in a set are immutable, which means we cannot change them. Some other immutable data types in Python are strings, tuples, and numbers such as integers and floats

## Creating a set

The syntax of a set is similar to other data structures like lists and dictionaries with minor differences. To create a set, we begin by writing a pair of curly brackets `{}`; inside the brackets, we separate the elements of the set by commas and a space(optional) just like we would do in a list.

![Syntax of a set](pictures/sets.png)

*Creating a set looks similar to creating a dictionary; you enclose a bunch of items within braces.*

(*Source*: Freecodecamp.org)

### Using the `set()` Constructor
Another way to create a set is using the `set()` function or constructor. For example, we could Create a set from a list, tuple or string using the `set()` constructor to implement this. The data structure will be converted to a set, removing duplicate elements.

![converting a list to a set](pictures/sets1.png)

```python
# Set
>>> {1, 2, 3, 4}
{1, 2, 3, 4}

# From a list
>>> set([1, 2, 3, 4])
{1, 2, 3, 4}

# From a tuple
>>> set((1, 2, 3, 4))
{1, 2, 3, 4}
```