# Introduction to sets in Python
In this lesson, we are going to learn about sets in the Python programing language.

A set is a collection of unordered elements that are unique. In Python, sets are extraordinary because they have no duplicate values or items, so we can utilize them to eliminate duplicate elements from lists and tuples effectively. In addition, the elements in a set are immutable, which means we cannot change them. Some other immutable data types in Python are strings, tuples, and numbers such as integers and floats

## Creating a set

The syntax of a set is similar to other data structures like lists and dictionaries with minor differences. To create a set, we begin by writing a pair of curly brackets `{}`; inside the brackets, we separate the elements of the set by commas and a space(optional) just like we would do in a list or by using the built-in set() function.

![Syntax of a set](pictures/sets.png)

*Creating a set looks similar to creating a dictionary; you enclose a bunch of items within braces.*

(*Source*: Freecodecamp.org)

A set can contain any number of elements regardless of type (integer, float, tuple, string etc). However, a set cannot have mutable elements like lists, sets or dictionaries as its elements.

```python
# set of integers
>>> my_set = {1, 2, 3}
>>> print(my_set)

# set of mixed datatypes
>>> my_set = {1.0, "Hello", (1, 2, 3)}
>>> print(my_set)

```

### Using the `set()` Constructor
Another way to create a set is using the `set()` function or constructor. For example, we could Create a set from a list, tuple or string using the `set()` constructor to implement this. The data structure will be converted to a set, removing duplicate elements.

![converting a list to a set](pictures/sets1.png)
(*Source*: Freecodecamp.org)

Examples of using a set() constructor.

```python
# defining a set
>>> {1, 2, 3, 4}
{1, 2, 3, 4}

# Converting a string to a set
>>> print set('abcd')
# prints
set(['a', 'c', 'b', 'd'])

# Converting a list to a set
>>> set([1, 2, 3, 4])
{1, 2, 3, 4}

# Converting a tuple to a set
>>> set((1, 2, 3, 4))
{1, 2, 3, 4}
```

>>> a = [1, 2, 2, 2, 2, 3, 4, 1, 4]
>>> set(a)
{1, 2, 3, 4}
## `Note:` If the elements in the `set()` has duplicate values, they will be removed to create the set.

example:

```python
>>> items = [1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 1, 4]
>>> set(items)
{1, 2, 3, 4}
```
## Common operations of sets in Python.

