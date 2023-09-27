# Recursion in Python

Welcome to the Recursion in Python guide! Recursion is a powerful technique in programming where a function calls itself to solve a problem. In this guide, we'll explore recursion through five examples of increasing complexity.

## What is Recursion?

Recursion is a programming technique where a function solves a problem by breaking it down into smaller, similar subproblems. Each recursive call works on a smaller instance of the problem until a base case is reached, at which point the recursion stops and the solutions are combined to solve the original problem.

## Example 1: Factorial Calculation

Let's start with a classic example - calculating the factorial of a number using recursion:

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

# Usage
result = factorial(5)
print(f"Factorial of 5 is {result}")
```

In this example, the `factorial` function calls itself with a smaller value (`n - 1`) until it reaches the base case (`n == 0`).

## Example 2: Fibonacci Sequence

The Fibonacci sequence is a famous recursive sequence where each number is the sum of the two preceding ones. Here's a recursive function to calculate Fibonacci numbers:

```python
def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n - 1) + fibonacci(n - 2)

# Usage
result = fibonacci(6)
print(f"The 6th Fibonacci number is {result}")
```

In this example, the `fibonacci` function calls itself twice, once for `n - 1` and once for `n - 2`, until it reaches the base cases (`n <= 1`).

## Example 3: Binary Search

Recursion is also useful for solving problems like binary search. Here's a recursive binary search function:

```python
def binary_search(arr, target, low, high):
    if low > high:
        return -1
    mid = (low + high) // 2
    if arr[mid] == target:
        return mid
    elif arr[mid] < target:
        return binary_search(arr, target, mid + 1, high)
    else:
        return binary_search(arr, target, low, mid - 1)

# Usage
my_list = [1, 3, 5, 7, 9]
target_value = 5
result = binary_search(my_list, target_value, 0, len(my_list) - 1)
print(f"Index of {target_value} in the list: {result}")
```

In this example, the `binary_search` function calls itself with narrowed search ranges until it finds the target or concludes that it's not in the list.

## Example 4: Tower of Hanoi

The Tower of Hanoi is a classic problem that involves moving disks from one peg to another while following specific rules. Here's a recursive solution:

```python
def tower_of_hanoi(n, source, auxiliary, target):
    if n == 1:
        print(f"Move disk 1 from {source} to {target}")
        return
    tower_of_hanoi(n - 1, source, target, auxiliary)
    print(f"Move disk {n} from {source} to {target}")
    tower_of_hanoi(n - 1, auxiliary, source, target)

# Usage
tower_of_hanoi(3, 'A', 'B', 'C')
```

In this example, the `tower_of_hanoi` function calls itself to solve smaller subproblems of moving fewer disks.

## Example 5: Recursive Backtracking (N-Queens Problem)

For a more advanced example, let's solve the N-Queens problem using recursive backtracking:

```python
def is_safe(board, row, col, n):
    # Check the column on the left
    for i in range(col):
        if board[row][i] == 1:
            return False

    # Check upper-left diagonal
    for i, j in zip(range(row, -1, -1), range(col, -1, -1)):
        if board[i][j] == 1:
            return False

    # Check lower-left diagonal
    for i, j in zip(range(row, n, 1), range(col, -1, -1)):
        if board[i][j] == 1:
            return False

    return True

def solve_n_queens(board, col, n):
    if col >= n:
        return True

    for i in range(n):
        if is_safe(board, i, col, n):
            board[i][col] = 1
            if solve_n_queens(board, col + 1, n):
                return True
            board[i][col] = 0

    return False

def print_solution(board):
    for row in board:
        print(" ".join(map(str, row)))

# Usage
n = 8  # Change this value to solve for different board sizes
chess_board = [[0] * n for _ in range(n)]
if solve_n_queens(chess_board, 0, n):
    print_solution(chess_board)
else:
    print("No solution exists")

```

In this example, we solve the N-Queens problem using recursive backtracking, a more complex form of recursion that explores multiple paths and unwinds when necessary to find a solution.

Recursion is a powerful tool in programming, allowing you to solve complex problems elegantly by breaking them down into simpler subproblems. As you become more comfortable with recursion, you'll find it a valuable tool in your coding toolkit.
