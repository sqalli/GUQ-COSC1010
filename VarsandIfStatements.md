# Variable Declaration and If Statements in Python

This README provides an introduction to variable declaration, if statements, and nested if statements in Python. It includes explanations and examples to help you understand these fundamental concepts.

## Table of Contents

- [Variable Declaration](#variable-declaration)
  - [Example 1: Declaring Variables](#example-1-declaring-variables)
  - [Example 2: Assigning Values to Variables](#example-2-assigning-values-to-variables)
- [If Statements](#if-statements)
  - [Example 1: Basic If Statement](#example-1-basic-if-statement)
  - [Example 2: If-Else Statement](#example-2-if-else-statement)
  - [Example 3: If-elif-else statement](#example-2-if-else-statement)
- [Nested If Statements](#nested-if-statements)
  - [Example: Nested If-Else](#example-nested-if-else)

## Variable Declaration

In Python, you can declare variables without specifying their data types explicitly. Variable names are case-sensitive and can contain letters, numbers, and underscores. 

### Example 1: Declaring Variables

```python
# Variable declaration
name = "Alice"
age = 30
```

### Example 2: Assigning Values to Variables

```python
# Assigning values to variables
x = 5
y = 10
```

## If Statements

If statements are used to make decisions in your code based on a condition. If the condition is true, the code block inside the if statement is executed.

### Example 1: Basic If Statement

```python
# Basic if statement
age = 25

if age < 18:
    print("You are underage.")
```

### Example 2: If-Else Statement

```python
# If-else statement
temperature = 28

if temperature > 30:
    print("It's hot outside.")
else:
    print("It's not too hot.")
```
### Example 3: If-elif-else statement

```python

score = 75

if score >= 90:
    print("A grade")
elif score >= 80:
    print("B grade")
elif score >= 70:
    print("C grade")
else:
    print("D grade")
```

In this example, we use the `elif` (short for "else if") statement to handle multiple conditions in a structured way. The code checks the `score` variable and prints the corresponding grade based on the score's value.

## Nested If Statements

The added example demonstrates the use of the `elif` statement to handle multiple conditions in an if-elif-else statement, providing more flexibility when making decisions based on varying conditions.
Nested if statements occur when you place an if statement inside another if statement. They are used to create more complex conditions.

### Example: Nested If-Else

```python
# Nested if-else statement
grade = 85

if grade >= 90:
    print("A grade")
else:
    if grade >= 80:
        print("B grade")
    else:
        print("C grade")
```

In this example, we use nested if-else statements to determine the grade based on the value of the `grade` variable.

Feel free to experiment with these examples to understand how variable declaration and if statements work in Python.

```

This README provides explanations and examples for variable declaration, if statements, and nested if statements in Python, with each topic clearly organized and formatted in Markdown for easy readability.
