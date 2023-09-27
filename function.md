# Introduction to Functions in Python

In this week, we will dive into the concept of functions in Python. Functions are essential building blocks in programming, allowing you to organize and reuse code efficiently. They help make your code more readable, modular, and easier to maintain.

## What is a Function?

A function is a named block of code that performs a specific task or set of tasks. Functions can take input data (called arguments or parameters), process it, and return a result. Functions are like mini-programs within your program, allowing you to break down complex tasks into smaller, more manageable pieces.

## Defining a Function

In Python, you can define a function using the `def` keyword followed by the function name, parentheses for parameters (if any), and a colon to start the function's code block. Here's a simple example:

```python
def greet(name):
    print(f"Hello, {name}!")
```

In this example, we defined a function called `greet` that takes one parameter, `name`, and prints a greeting message with the provided name.

## Example 1: Basic Function

Let's start with a basic function that calculates the square of a number:

```python
def square(x):
    result = x * x
    return result

# Usage
num = 5
print(f"The square of {num} is {square(num)}")
```

This function takes an argument `x`, calculates its square, and returns the result.

## Example 2: Default Arguments

You can also specify default values for function parameters:

```python
def power(base, exponent=2):
    result = base ** exponent
    return result

# Usage
print(power(2))  # Default exponent is 2
print(power(2, 3))  # Custom exponent: 2^3
```

Here, the `power` function has a default exponent value of 2, but you can provide a custom exponent if needed.

## Example 3: Variable Number of Arguments

Python allows you to define functions that accept a variable number of arguments using `*args`:

```python
def sum_all(*args):
    total = sum(args)
    return total

# Usage
print(sum_all(1, 2, 3, 4, 5))
```

The `*args` syntax collects all provided arguments into a tuple, making it easy to work with a variable number of inputs.

## Example 4: Keyword Arguments

You can use keyword arguments to make your function calls more explicit:

```python
def show_info(name, age, city):
    print(f"Name: {name}, Age: {age}, City: {city}")

# Usage
show_info(age=30, name="Alice", city="New York")
```

This allows you to pass arguments out of order and makes your code more readable.

## Example 5: Recursive Function

A recursive function is one that calls itself. Here's a simple recursive function to calculate the factorial of a number:

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

# Usage
print(factorial(5))
```

Recursive functions can be a powerful way to solve problems that can be broken down into smaller, similar sub-problems.

## Example 6: Lambda Functions

Lambda functions, also known as anonymous functions, are short, one-liner functions defined using the `lambda` keyword:

```python
square = lambda x: x * x

# Usage
print(square(4))
```

Lambda functions are often used for simple, throwaway operations.

## Example 7: Function with Docstring

It's a good practice to include docstrings in your functions to provide documentation on what the function does. Here's an example with a docstring:

```python
def add(a, b):
    """
    This function adds two numbers and returns the result.
    """
    result = a + b
    return result

# Usage
print(add(3, 5))
```

Docstrings are helpful for understanding the purpose of a function, especially in larger codebases.

## Example 8: Function with Multiple Return Values

Python functions can return multiple values as a tuple. Let's create a function that calculates both the sum and product of two numbers:

```python
def calculate_sum_and_product(x, y):
    """
    Calculate the sum and product of two numbers.
    """
    summation = x + y
    product = x * y
    return summation, product

# Usage
result = calculate_sum_and_product(2, 3)
print(f"Sum: {result[0]}, Product: {result[1]}")
```

Here, the function returns a tuple with two values, which we can unpack as needed.

## Example 9: Function with a Global Variable

In this example, we'll use a global variable within a function:

```python
global_variable = 10

def modify_global():
    global global_variable
    global_variable += 5

# Usage
modify_global()
print(global_variable)
```

By using the `global` keyword, we can modify a global variable from within a function.

That concludes our introduction to functions in Python! They are a fundamental concept that you will use extensively in your coding journey. Functions help you write clean, organized, and reusable code. As you progress, you'll learn more about advanced topics and best practices for using functions effectively in Python. Happy coding!
