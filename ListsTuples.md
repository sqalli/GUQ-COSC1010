
# COSC1010 Data Containers - Lists and Tuples

Welcome to Week 7 of the COSC1010 Class. In this session, we will explore data containers in Python, with a specific focus on lists and tuples. By the end of this class, you will understand the differences between lists and tuples, know how to create and manipulate them, and be able to apply them in practical scenarios.

## Table of Contents

- [Data Containers: Lists and Tuples](#data-containers-lists-and-tuples)
- [Lists](#lists)
  - [Creating Lists](#creating-lists)
  - [Accessing and Modifying Lists](#accessing-and-modifying-lists)
- [Tuples](#tuples)
  - [Creating Tuples](#creating-tuples)
  - [Immutability of Tuples](#immutability-of-tuples)
- [In-Class Practice](#in-class-practice)

## Lists

### Creating Lists

In Python, a list is an ordered collection of items, which can be of different data types. Lists are versatile and commonly used in various programming tasks. Here's how to create a list:

```python
fruits = ["apple", "banana", "cherry"]
```

### Accessing and Modifying Lists

You can access and modify elements within a list using indexing and slicing:

```python
# Accessing elements
first_fruit = fruits[0]  # Access the first item (index 0)

# Modifying elements
fruits[1] = "kiwi"  # Change the second item to "kiwi"
```

Lists can also be extended, reversed, sorted, and much more.

## Tuples

### Creating Tuples

A tuple is similar to a list, but with one key difference: tuples are immutable, meaning their elements cannot be changed once defined. Here's how to create a tuple:

```python
dimensions = (10, 5, 8)
```

### Immutability of Tuples

Unlike lists, tuples cannot be modified:

```python
# This will raise an error
dimensions[0] = 12
```

Tuples are commonly used for data that should not be changed, such as coordinates.

## In-Class Practice

Now, let's practice working with lists and tuples:

1. Write a Python function that takes a list of numbers as input and returns the sum of all the numbers in the list.

## Conclusion

In this session, we covered data containers in Python, with a focus on lists and tuples. We also focused on the basic sorting algorithms including selection sort, buble sort, and insertion sort.
To conclude Lists are versatile and mutable and are the fundamentals of algorithms especially sorting. Tuples however are immutable and often used for unchangeable data. Practice these concepts, and you'll be better equipped to work with data structures in Python.

If you have any questions or need assistance, feel free to reach out at mt1516@georgetown.edu
