# Section 1: Quick Overview

## Lists
Lists are ordered collections of items that can be changed. They are defined using square brackets.

### Creating and Accessing Lists
```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # Output: apple
```

### List Methods
- `append()`: Adds an item to the end of the list.
- `remove()`: Removes the first occurrence of a specified item.
- `sort()`: Sorts the items in the list.

## Tuples
Tuples are similar to lists but are immutable (cannot be changed). They are defined using parentheses.

### Creating and Accessing Tuples
```python
coordinates = (10, 20)
print(coordinates[1])  # Output: 20
```

### Tuple Methods
- `count()`: Returns the number of times a specified value occurs in a tuple.
- `index()`: Returns the index of the first occurrence of a specified value.

## Dictionaries
Dictionaries are collections of key-value pairs. They are defined using curly braces.

### Creating and Accessing Dictionaries
```python
person = {"name": "Alice", "age": 25}
print(person["name"])  # Output: Alice
```

### Dictionary Methods
- `get()`: Returns the value for a specified key.
- `keys()`: Returns a list of all the keys in the dictionary.

## Sets
Sets are unordered collections of unique items. They are defined using curly braces.

### Creating and Accessing Sets
```python
unique_numbers = {1, 2, 3, 4, 5}
print(unique_numbers)  # Output: {1, 2, 3, 4, 5}
```

### Set Methods
- `add()`: Adds an item to the set.
- `remove()`: Removes a specified item from the set.
