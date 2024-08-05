# Importing Modules

## Overview
In Python, you can use the `import` statement to include the functionality of a module in your code. This allows you to access functions, classes, and variables defined in that module.

## Syntax
```python
import module_name
```

## Example
```python
import math

result = math.sqrt(16)  # result will be 4.0
print(result)
```

## Importing Specific Functions
You can also import specific functions from a module.
```python
from math import pi

print(pi)  # Output: 3.141592653589793
```

## Creating and Importing Custom Modules
You can create your own modules by saving Python code in a `.py` file. For example, if you have a file named `my_module.py` with a function `greet()`, you can import it as follows:
```python
import my_module

my_module.greet("Alice")
```
