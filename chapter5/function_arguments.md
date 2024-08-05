# Function Arguments

## Overview
Function arguments allow you to pass values to functions. Python supports several types of arguments.

## Types of Arguments

1. **Positional Arguments**: These are the most common type of arguments. They are assigned to parameters based on their position.
   ```python
   def add(a, b):
       return a + b

   result = add(5, 3)  # 5 is assigned to a, 3 is assigned to b
   ```

2. **Keyword Arguments**: These arguments are passed by explicitly stating the parameter name.
   ```python
   result = add(b=3, a=5)  # Order does not matter
   ```

3. **Default Arguments**: You can provide default values for parameters.
   ```python
   def greet(name, message="Hello"):
       print(message + ", " + name + "!")

   greet("Alice")  # Output: Hello, Alice!
   ```

4. **Variable-Length Arguments**: You can use `*args` and `**kwargs` to pass a variable number of arguments.
   ```python
   def print_numbers(*args):
       for number in args:
           print(number)

   print_numbers(1, 2, 3, 4)  # Output: 1 2 3 4
   
