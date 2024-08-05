# Creating Packages

## Overview
A package is a way of organizing related modules in a directory hierarchy. It allows you to structure your code in a more manageable way.

## Creating a Package
To create a package, follow these steps:
1. Create a directory for your package.
2. Inside that directory, create an `__init__.py` file (this file can be empty).
3. Add your module files (e.g., `module1.py`, `module2.py`) to the package directory.

### Example
Suppose you have the following directory structure:
```
my_package/
    __init__.py
    module1.py
    module2.py
```

You can import modules from your package as follows:
```python
from my_package import module1
from my_package.module2 import some_function
```

## Using Packages
Once you have created a package, you can use it in your Python scripts just like any other module.
```python
import my_package.module1
my_package.module1.some_function()
```
