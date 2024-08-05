# Return Values

## Overview
In Python, functions can return values using the `return` statement. This allows you to send data back to the caller of the function.

## Syntax
```python
def function_name(parameters):
    # code to execute
    return value
```

## Example
```python
def square(number):
    return number * number

result = square(4)  # result will be 16
print(result)
```

## Multiple Return Values
Functions can also return multiple values as a tuple.
```python
def min_max(numbers):
    return min(numbers), max(numbers)

minimum, maximum = min_max([1, 2, 3, 4, 5])  # minimum = 1, maximum = 5
print(minimum, maximum)
```
