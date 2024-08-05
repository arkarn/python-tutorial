
# Mastering Control Flow in Python

In the Python scripts we've encountered so far, execution has followed a top-down sequence without deviation. However, real-world scenarios often require the program to make decisions and execute different paths based on varying conditions. For instance, you might want the program to display 'Good Morning' or 'Good Evening' depending on the current time.

This flexibility is achieved through control flow statements, which include `if`, `for`, and `while`.

## The `if` Statement

The `if` statement allows the program to evaluate a condition and execute a block of code if the condition is true. Optionally, it can execute another block of code if the condition is false.

Example (save as `check_age.py`):

```python
# Filename: check_age.py
age = int(input("Enter your age: "))

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

**Explanation:**

In this program, we prompt the user to input their age. We then use an `if` statement to check if the age is 18 or older. If true, it prints a message stating the user is an adult; otherwise, it prints that the user is a minor. Notice how indentation is crucial to indicate which statements belong to the `if` block and the `else` block.

### Nested `if` Statements

You can nest `if` statements inside other `if` blocks:

```python
# Filename: nested_if.py
num = int(input("Enter a number: "))

if num > 0:
    print("The number is positive.")
    if num % 2 == 0:
        print("It's also even.")
else:
    print("The number is non-positive.")
```

### The `elif` Clause

The `elif` (else-if) clause allows for multiple conditions to be checked in sequence:

```python
# Filename: grading.py
score = int(input("Enter your score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
else:
    print("Grade: D or lower")
```

## The `while` Loop

The `while` loop enables repeated execution of a block of code as long as a specified condition remains true.

Example (save as `countdown.py`):

```python
# Filename: countdown.py
count = 5

while count > 0:
    print(count)
    count -= 1
print("Blast off!")
```

**Explanation:**

This script counts down from 5 to 1, then prints "Blast off!". The loop continues to run as long as `count` is greater than 0. Each iteration decreases `count` by 1.

### Using `else` with `while`

The `else` clause can be used with `while` to execute a block of code once the loop condition becomes false:

```python
# Filename: guess_number.py
secret_number = 7
attempts = 0

while attempts < 3:
    guess = int(input("Guess the number: "))
    if guess == secret_number:
        print("Congratulations! You've guessed correctly.")
        break
    attempts += 1
else:
    print("Sorry, you've used all attempts.")
```

## The `for` Loop

The `for` loop iterates over a sequence (e.g., list, tuple, string) and executes a block of code for each item in the sequence.

Example (save as `print_numbers.py`):

```python
# Filename: print_numbers.py
for num in range(1, 6):
    print(num)
```

**Explanation:**

This script prints numbers from 1 to 5. The `range(1, 6)` function generates a sequence from 1 to 5, and the loop iterates over this sequence, printing each number.

### The `break` Statement

The `break` statement terminates the loop prematurely, regardless of the loop's condition.

Example (save as `break_example.py`):

```python
# Filename: break_example.py
for letter in "python":
    if letter == 'h':
        break
    print(letter)
```

**Explanation:**

This script prints each letter in the word "python" until it encounters 'h', at which point it exits the loop.

### The `continue` Statement

The `continue` statement skips the rest of the code inside the current loop iteration and moves to the next iteration.

Example (save as `continue_example.py`):

```python
# Filename: continue_example.py
for num in range(1, 6):
    if num == 3:
        continue
    print(num)
```

**Explanation:**

This script prints numbers from 1 to 5, skipping the number 3.

## Summary

We've explored the essential control flow mechanisms in Python: `if`, `while`, and `for` loops, along with their associated `break` and `continue` statements. Mastery of these constructs is crucial as they are fundamental to controlling the execution flow of your programs.

Next, we'll delve into creating and using functions to further enhance our programming capabilities.
