# Chapter 2: Basic Syntax and Data Types

## Variables and Data Types
In Python, variables are used to store data values. Python has various data types, including:
- **Integers**: Whole numbers, e.g., `5`, `-3`.
- **Floats**: Decimal numbers, e.g., `3.14`, `-0.001`.
- **Strings**: Text data, e.g., `"Hello, World!"`.
- **Booleans**: Represents `True` or `False`.

### Declaring Variables
You can declare a variable by simply assigning a value to it:
```python
x = 5
name = "Alice"
is_active = True
```

## Basic Operators
Python supports several operators for performing operations on variables and values.

### Arithmetic Operators
- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)
- Modulus (`%`)

### Comparison Operators
- Equal to (`==`)
- Not equal to (`!=`)
- Greater than (`>`)
- Less than (`<`)

### Logical Operators
- And (`and`)
- Or (`or`)
- Not (`not`)

## Input and Output
You can use the `input()` function to get user input and the `print()` function to display output.

### Example
```python
name = input("Enter your name: ")
print("Hello, " + name + "!")
```

## Control Structures

### Conditional Statements
Python uses `if`, `elif`, and `else` statements to control the flow of the program based on conditions.

### Example
```python
age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

### Loops
You can use `for` and `while` loops to iterate over sequences or execute a block of code multiple times.

### Example of a For Loop
```python
for i in range(5):
    print(i)
```

### Example of a While Loop
```python
count = 0
while count < 5:
    print(count)
    count += 1
