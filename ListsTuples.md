
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
```python
def calculate_sum(numbers):
    total = 0  # Initialize a variable to store the sum

    for number in numbers:
        total += number  # Add each number to the total

    return total  # Return the sum

# Example usage:
numbers = [1, 2, 3, 4, 5]
result = calculate_sum(numbers)
print("The sum of the numbers is:", result)

```
2. Implement the Selection Sort algorithm in Python. The algorithm works by repeatedly finding the minimum element from the unsorted part of the list and putting it at the beginning. Test your implementation on a list of integers.
```python
def selection_sort(arr):
    for i in range(len(arr)):
        min_idx = i
        for j in range(i + 1, len(arr)):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]

# Example usage:
arr = [64, 25, 12, 22, 11]
selection_sort(arr)
print("Sorted array:", arr)
```
3. Implement the Bubble Sort algorithm in Python. Bubble Sort repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. Continue this process until the list is sorted. Test your implementation on a list of integers.
```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n - i - 1):
            if arr[j] > arr[j + 1]:
                arr[j], arr[j + 1] = arr[j + 1], arr[j]

# Example usage:
arr = [64, 34, 25, 12, 22, 11, 90]
bubble_sort(arr)
print("Sorted array:", arr)
```
4. Implement the Insertion Sort algorithm in Python. Insertion Sort builds the final sorted array one item at a time, inserting each element into its correct position. Test your implementation on a list of strings.
```python
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        while j >= 0 and key < arr[j]:
            arr[j + 1] = arr[j]
            j -= 1
        arr[j + 1] = key

# Example usage:
arr = ["apple", "banana", "kiwi", "cherry", "date"]
insertion_sort(arr)
print("Sorted array:", arr)
```   

## Conclusion

In this session, we covered data containers in Python, with a focus on lists and tuples. We also focused on the basic sorting algorithms including selection sort, buble sort, and insertion sort.
To conclude Lists are versatile and mutable and are the fundamentals of algorithms especially sorting. Tuples however are immutable and often used for unchangeable data. Practice these concepts, and you'll be better equipped to work with data structures in Python.

If you have any questions or need assistance, feel free to reach out at mt1516@georgetown.edu
