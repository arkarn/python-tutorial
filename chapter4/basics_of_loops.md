# Loops: Quick Overview

## Overview
Loops are used to execute a block of code repeatedly. In Python, there are two primary types of loops: `for` loops and `while` loops.

## For Loops
A `for` loop is used to iterate over a sequence (like a list, tuple, or string).

### Syntax
```python
for item in sequence:
    # code to execute for each item
```

### Example
```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

## While Loops
A `while` loop continues to execute as long as a specified condition is true.

### Syntax
```python
while condition:
    # code to execute while condition is true
```

### Example
```python
count = 0
while count < 5:
    print(count)
    count += 1
```
