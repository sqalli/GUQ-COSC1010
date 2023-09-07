# Python Reserved Words

This README provides a comprehensive overview of reserved words in Python, categorized into different types. Reserved words are special keywords that have predefined meanings in the Python language and cannot be used as identifiers (variable names, function names, etc.).

## Table of Contents

- [Introduction](#introduction)
- [Keywords](#keywords)
  - [Control Flow Keywords](#control-flow-keywords)
  - [Function Definition Keywords](#function-definition-keywords)
  - [Class Definition Keywords](#class-definition-keywords)
- [Built-in Constants](#built-in-constants)
  - [Boolean Constants](#boolean-constants)
  - [None](#none)
- [Built-in Functions](#built-in-functions)
  - [Print](#print)
  - [Len](#len)
  - [Type](#type)
- [Conclusion](#conclusion)

## Introduction

Python has a set of reserved words that serve specific purposes in the language. These reserved words are not to be used as identifiers for variables, functions, classes, or modules. Attempting to use them as identifiers will result in a `SyntaxError`. Understanding and respecting Python's reserved words is essential for writing correct and readable code.

## Keywords

Python keywords are used to define the syntax and structure of the language. They control the flow of code execution and provide the foundation for writing structured Python programs.

### Control Flow Keywords

Python includes keywords for control flow, such as `if`, `else`, and `while`, which are used to create conditional statements and loops.

**Examples**:

```python
# 'if' statement
if condition:
    print("This is an 'if' statement.")
else:
    print("This is the 'else' block of the 'if' statement.")

# 'while' loop
count = 0
while count < 5:
    print(f"Count is {count}")
    count += 1
```

### Function Definition Keywords

Python has keywords for defining functions, including `def`, which is used to declare a new function.

**Examples**:

```python
# Function definition
def greet(name):
    print(f"Hello, {name}!")

# Function call
greet("Alice")
```

## Built-in Constants

Python includes several built-in constants that represent fixed values with predefined meanings. These constants are used in various contexts and have specific roles in Python programming.

### Boolean Constants

Python has two Boolean constants, `True` and `False`, which represent the Boolean values of true and false, respectively.

**Examples**:

```python
# Boolean constants
is_true = True
is_false = False
```

### None

The `None` constant represents the absence of a value or a null value in Python. It is often used to initialize variables or indicate missing or empty data.

**Examples**:

```python
# Using None
my_variable = None
```

## Built-in Functions

Python provides a wide range of built-in functions that can be used to perform various operations. These functions are available for use without the need for explicit definitions.

### Print

The `print()` function is used to display text or variables to the console. It is a fundamental tool for debugging and providing output in Python programs.

**Examples**:

```python
# Using the 'print()' function
print("Hello, World!")

my_list = [1, 2, 3]
print(my_list)
```

### Len

The `len()` function is used to determine the length or number of elements in a sequence, such as a string, list, or tuple.

**Examples**:

```python
# Using the 'len()' function
my_string = "Python"
length = len(my_string)  # 'length' is now 6

my_list = [1, 2, 3, 4, 5]
list_length = len(my_list)  # 'list_length' is now 5
```

### Type

The `type()` function is used to determine the data type of an object or variable. It is particularly useful when working with dynamic typing in Python.

**Examples**:

```python
# Using the 'type()' function
value = 42
data_type = type(value)  # 'data_type' is now <class 'int'>

my_list = [1, 2, 3]
data_type_list = type(my_list)  # 'data_type_list' is now <class 'list'>
```

## Conclusion

Python's reserved words, including keywords, constants, and built-in functions, are an integral part of the language. Understanding their roles and using them appropriately is crucial for writing clean and effective Python code.
```
