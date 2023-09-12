# Week 4: Loops

## I. Introduction to Loops
Loops in programming are used to automate repetitive tasks by repeating a set of instructions multiple times. 
There are two main types of loops in Python: `for` loops and `while` loops.

## II. Types of Loops in Python
Python supports two primary loop types:
- `for` loops: Used for iterating over a sequence (e.g., lists, strings).
- `while` loops: Used for executing a block of code as long as a certain condition is met.

## III. `for` Loops
### Basic Structure
```python
for element in iterable:
    # Code to be repeated for each element
```
- `element`: A variable that takes on each value in the iterable.
- `iterable`: The sequence to loop through.

### Examples
- Iterating over lists and strings.
- Using the `range()` function to create sequences for looping.
- Using `enumerate()` to loop through elements and indices.
Certainly! Here are some simple `for` loop examples in Python with different arguments provided to the loop:

#### Example 1: Looping through a List
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
Output:
```
apple
banana
cherry
```

#### Example 2: Looping through a Range
```python
for num in range(1, 6):
    print(num)
```
Output:
```
1
2
3
4
5
```

#### Example 3: Looping through a String
```python
word = "Python"
for letter in word:
    print(letter)
```
Output:
```
P
y
t
h
o
n
```

#### Example 4: Looping with the `enumerate()` Function
```python
colors = ["red", "green", "blue"]
for index, color in enumerate(colors):
    print(f"Color {index + 1}: {color}")
```
Output:
```
Color 1: red
Color 2: green
Color 3: blue
```

### Example 5: Looping with a Step Value
```python
for i in range(0, 10, 2):
    print(i)
```
Output:
```
0
2
4
6
8
```
### Application Example: 1 

Find the maximum of `l = [5, 3, 12, 10, 27, 9, 15]`

### Example 6: Nested `for` loops

In Python, you can use nested loops, which are loops inside other loops, to perform more complex repetitive tasks. Nested loops allow you to iterate over elements in multiple dimensions, such as rows and columns in a matrix.

What do you think the following code provide you

```python
for i in range(1, 11):
    for j in range(1, 11):
        result = i * j
        print(f"{i} x {j} = {result}")
    print()  # Add a newline after each row
```

### Application Example 2: Displaying a Triangle

Write a Python program that uses `for` loops to display a triangle pattern. The program should take an integer input from the user to determine the height of the triangle and then print the triangle pattern accordingly.

Here's the pattern you need to create:
```
Enter the height of the triangle: 5

*
**
***
****
*****
```

#### Instructions:

1. Prompt the user to enter the height of the triangle using `input()`. Make sure to convert the input to an integer.

2. Use nested `for` loops to iterate through the rows and columns of the triangle.

3. The outer loop controls the rows, and the inner loop controls the columns.

4. Print an asterisk (`*`) for each column in each row. The number of asterisks in each row should be equal to the row number.

5. Ensure that there is a newline character (`\n`) at the end of each row to create the triangle shape.

#### Example Output:

```
Enter the height of the triangle: 5

*
**
***
****
*****
```

#### Constraints:

- The height of the triangle should be a positive integer.

#### Hint:

- You can use the `range()` function to control the number of iterations in the `for` loops.

## IV. `while` Loops
### Basic Structure
```python
while condition:
    # Code to be repeated as long as the condition is True
```
- `condition`: A boolean expression that determines when to exit the loop.
- Important: Ensure a terminating condition to avoid infinite loops.

### Control Statements
- `break`: Exits the loop prematurely.
- `continue`: Skips the current iteration and moves to the next one.

## V. Loop Control Statements
## `break` Statement
- Used to exit a loop prematurely when a certain condition is met.

## `continue` Statement
- Used to skip the current iteration and move to the next one within the loop.

## Examples:
Here are Python examples to visualize the concepts of `while` loops, including an example that explains the `break` and `continue` concepts, presented in Markdown format:
In Python, a `while` loop is used to repeatedly execute a block of code as long as a specified condition is `True`. Here are examples to illustrate different aspects of `while` loops.

### Example 1: Simple While Loop

This example demonstrates a simple `while` loop that counts from 1 to 5.

```python
counter = 1
while counter <= 5:
    print(counter)
    counter += 1
```

**Output:**

```
1
2
3
4
5
```

### Example 2: Using the `break` Statement

The `break` statement is used to exit a `while` loop prematurely. In this example, the loop stops when the value of `x` becomes greater than 3.

```python
x = 1
while x <= 5:
    print(x)
    if x > 3:
        break
    x += 1
```

**Output:**

```
1
2
3
4
```

### Example 3: Using the `continue` Statement

The `continue` statement is used to skip the current iteration of a loop and continue with the next one. In this example, the loop skips printing even numbers.

```python
x = 1
while x <= 5:
    if x % 2 == 0:
        x += 1
        continue
    print(x)
    x += 1
```

**Output:**

```
1
3
5
```

### Example 4: Infinite Loop with `while True`

In some cases, you may want to create an infinite loop using `while True`. You can exit this loop using a `break` statement when a specific condition is met.

```python
while True:
    user_input = input("Enter 'q' to quit: ")
    if user_input == 'q':
        break
    print("You entered:", user_input)
```

In this example, the loop continues until the user enters 'q'.

### Practice Example 1: Infinite Loop with `while True`

Write a program that keeps on asking the user about their grade until they enter a negative grade. The program should be able to identify the minimum and maximum grades among all the entered grades.

## V. Tips and Best Practices
- Write clean and efficient loops.
- Choose meaningful variable names.
- Enhance code readability with comments.

## VI. Homework Assignment (See canvas)
- Refer to Canvas for HW2. The second homework covers conditions as well as loops as the founding elements of programming in Python.
