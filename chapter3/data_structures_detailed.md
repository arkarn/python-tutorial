# Section 2: Data Structures

Data structures are fundamental elements that help us organize and store data in various ways. In Python, there are several built-in data structures that simplify managing collections of data. The primary built-in data structures are lists, tuples, dictionaries, and sets. Each serves a specific purpose and has its own characteristics.

## List

A `list` is a versatile data structure in Python that holds an ordered sequence of items. Imagine a list as a to-do list where each task is an item. In Python, we use square brackets to define a list and separate items with commas.

Lists are **mutable**, meaning you can change their contents by adding, removing, or modifying items. This flexibility is useful for many tasks.

**Example:**

```python
# Create a list of fruits
fruits = ['apple', 'banana', 'cherry']

# Add a fruit to the list
fruits.append('date')

# Remove a fruit from the list
del fruits[1]  # Removes 'banana'

# Sort the list alphabetically
fruits.sort()

# Print the list
print(fruits)
```

**Output:**

```
['apple', 'cherry', 'date']
```

**Explanation:**

In this example, `fruits` is a list that initially contains three items. We used the `append` method to add 'date' to the end and the `del` statement to remove 'banana'. The `sort` method sorts the list in alphabetical order.

## Tuple

A `tuple` is another data structure that groups together multiple values. Unlike lists, tuples are **immutable**, meaning once created, their contents cannot be changed. They are defined using parentheses, and items are separated by commas.

**Example:**

```python
# Define a tuple of colors
colors = ('red', 'green', 'blue')

# Access items in the tuple
print(colors[1])  # Output: 'green'

# Nested tuple example
nested_tuple = ('a', ('b', 'c'), 'd')
print(nested_tuple[1][1])  # Output: 'c'
```

**Output:**

```
green
c
```

**Explanation:**

In the example, `colors` is a tuple. We accessed an item using its index. Tuples can also be nested, as shown with `nested_tuple`.

## Dictionary

A `dictionary` in Python is a collection of key-value pairs. Think of it as an address book where each name (key) is associated with contact details (value). Keys must be unique and immutable, while values can be of any type.

Dictionaries are created using curly braces, with key-value pairs separated by commas and colons.

**Example:**

```python
# Create a dictionary of contacts
contacts = {
    'John': '555-1234',
    'Jane': '555-5678'
}

# Add a new contact
contacts['Doe'] = '555-8765'

# Remove a contact
del contacts['Jane']

# Access a contact's number
print(contacts['John'])  # Output: '555-1234'
```

**Output:**

```
555-1234
```

**Explanation:**

The `contacts` dictionary initially contains two key-value pairs. We added a new pair with 'Doe' and removed 'Jane'. Accessing a contact’s number is done using the key.

## Set

A `set` is an unordered collection of unique items. Sets are useful when you care only about the presence of items, not their order or frequency. They support operations like membership tests, unions, intersections, and differences.

**Example:**

```python
# Create a set of countries
countries = {'USA', 'Canada', 'Mexico'}

# Check membership
print('USA' in countries)  # Output: True

# Add a new country
countries.add('Brazil')

# Remove a country
countries.discard('Canada')

# Find the intersection with another set
other_countries = {'Brazil', 'Argentina'}
print(countries & other_countries)  # Output: {'Brazil'}
```

**Output:**

```
True
{'Brazil'}
```

**Explanation:**

In this example, `countries` is a set. We checked if 'USA' is in the set, added 'Brazil', and removed 'Canada'. We also found the intersection with another set `other_countries`.

## Sequence

Sequences in Python include lists, tuples, and strings. They share some common features:

- **Membership tests** using `in` and `not in`.
- **Indexing** to access individual elements.
- **Slicing** to extract parts of the sequence.

**Example:**

```python
# Create a list
numbers = [10, 20, 30, 40, 50]

# Access items by index
print(numbers[0])  # Output: 10
print(numbers[-1]) # Output: 50

# Slice the list
print(numbers[1:4])  # Output: [20, 30, 40]

# Slice with step
print(numbers[::2])  # Output: [10, 30, 50]
```

**Output:**

```
10
50
[20, 30, 40]
[10, 30, 50]
```

**Explanation:**

We accessed elements by index, used slicing to get sublists, and applied a step value in slicing to skip elements.

## Set Theory in Python

Sets in Python align well with basic set theory concepts like unions, intersections, and differences. For instance, you can perform these operations using Python set methods and operators.

**Example:**

```python
# Define two sets
set1 = {1, 2, 3, 4}
set2 = {3, 4, 5, 6}

# Union
print(set1 | set2)  # Output: {1, 2, 3, 4, 5, 6}

# Intersection
print(set1 & set2)  # Output: {3, 4}

# Difference
print(set1 - set2)  # Output: {1, 2}
```

**Output:**

```
{1, 2, 3, 4, 5, 6}
{3, 4}
{1, 2}
```

**Explanation:**

Here, we used set operations to find the union, intersection, and difference between two sets.

## References and Binding

When you create a variable in Python, it holds a reference to an object, not the object itself. This means if you assign one variable to another, they both reference the same object.

**Example:**

```python
# Create a list
original_list = [1, 2, 3]

# Assign to a new variable
alias_list = original_list

# Modify the original list
alias_list.append(4)

# Both variables reflect the change
print(original_list)  # Output: [1, 2, 3, 4]
print(alias_list)     # Output: [1, 2, 3, 4]
```

**Output:**

```
[1, 2, 3, 4]
[1, 2, 3, 4]
```

**Explanation:**

`alias_list` is a reference to `original_list`, so changes to one affect the other. To create an independent copy, use slicing or the `copy` module.

## More About Strings

Strings in Python are objects and come with a range of methods. These methods allow you to perform various operations on strings, such as checking their content or manipulating them.

**Example:**

```python
# Create a string
text = "hello world"

# Check if it starts with a substring
print(text.startswith("hello"))  # Output: True

# Find the position of a substring
print(text.find("world"))  # Output: 6

# Join a list of strings into a single string
words = ['join', 'these', 'words']
print(' '.join(words))  # Output: 'join these words'
```

**Output:**

```
True
6
join these words
```

**Explanation:**

We used string methods like `startswith`, `find`, and `join` to manipulate and examine string data.

## Summary

We’ve covered several essential data structures in Python: lists, tuples, dictionaries, and sets. Understanding these will help you manage and process data effectively in your programs. As you advance, you'll apply these data structures to solve more complex problems and design robust Python applications.
