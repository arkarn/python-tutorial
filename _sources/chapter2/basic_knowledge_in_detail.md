# Section 2: Python Basics

## Understanding Comments

_Comments_ are annotations in your code that follow the `#` symbol. They serve as notes to clarify what your code does, either for yourself or others who read your code later.

For example:

```python
print('hello world') # This line prints 'hello world'
```

or:

```python
# This line prints 'hello world'
print('hello world')
```

Comments are invaluable for:

- Explaining assumptions and decisions
- Providing context for critical details
- Addressing issues or solutions in your code

[**Code shows how; comments explain why**](http://www.codinghorror.com/blog/2006/12/code-tells-you-how-comments-tell-you-why.html). This practice helps anyone reading the code, including your future self.

## Literal Constants

Literal constants are values you use directly in your code. Examples include integers like `5`, floating-point numbers such as `1.23`, and strings like `'This is a string'`.

The term _literal_ refers to these values being used as they are, without modification. For instance, `2` is always the number `2` and is constant because its value remains unchanged.

## Working with Numbers

In Python, numbers are categorized primarily into two types: integers and floats.

- **Integers** are whole numbers, such as `2`.
- **Floats** represent numbers with decimal points, like `3.23` or `52.3E-4`, where `E` denotes powers of 10. For instance, `52.3E-4` equals `52.3 * 10^-4`.

> **Tip for Experienced Programmers:**
>
> Python does not have a separate `long` type; `int` can handle integers of any size.

## Strings

Strings are sequences of characters and are fundamental in most Python programs. 

### Single and Double Quotes

Strings can be enclosed in single quotes (`'Example'`) or double quotes (`"Example"`). Both behave similarly:

```python
'Hello, world!'
"Hello, world!"
```

### Triple Quotes

For multi-line strings, use triple quotes (`'''` or `"""`):

```python
'''This is a multi-line string.
It spans multiple lines.
"What's your name?" I asked.'''
```

### String Immutability

Strings in Python are immutable, meaning once created, they cannot be changed. This immutability has advantages, which we'll explore in future examples.

> **Note for C/C++ Programmers:**
> 
> Python doesn’t have a `char` data type—strings cover all needs.

### The `format()` Method

The `format()` method allows for constructing strings from other variables:

Save the following code as `str_format.py`:

```python
office = Grab
name = 'Ashish'

print('{0} works at {1}'.format(name, age))
print('Why is {0} dancing?'.format(name))
```

Output:

```
Ashish works at Grab
Why is Ashish dancing?
```

**How It Works:**

The `format()` method replaces placeholders like `{0}` with corresponding arguments. You can also use named placeholders:

```python
print('{name} was {age} years old when he wrote this book'.format(name=name, age=age))
```

From Python 3.6 onwards, you can use f-strings for even more concise formatting:

```python
print(f'{name} was {age} years old when he wrote this book')
print(f'Why is {name} playing with that python?')
```

### Escape Sequences

To include special characters in strings, use escape sequences. For example, to include a single quote inside a single-quoted string:

```python
'What\'s your name?'
```

Or use double quotes:

```python
"What's your name?"
```

Escape sequences like `\n` for new lines and `\t` for tabs are also useful:

```python
'This is the first line\nThis is the second line'
```

For raw strings where escape sequences are not processed, prefix with `r`:

```python
r"Newlines are indicated by \n"
```

> **Note for Regex Users:**
> 
> Use raw strings for regular expressions to avoid excessive escaping.

## Variables

Variables are placeholders for storing and manipulating data. Unlike literals, their values can change throughout the program’s execution.

## Naming Identifiers

Variables, also known as identifiers, must follow these rules:

- Begin with a letter (A-Z, a-z) or underscore (`_`).
- Subsequent characters can be letters, underscores, or digits (0-9).
- Identifiers are case-sensitive, meaning `variable` and `Variable` are different.

Valid identifiers: `i`, `name_2_3`. Invalid identifiers: `2things`, `this is spaced out`, `my-name`, and `>a1b2_c3`.

## Data Types

Variables can store values of various types, such as numbers and strings. We will explore custom types through classes in later chapters.

## Everything is an Object

In Python, everything is treated as an object, including numbers, strings, and functions.

> **For Object-Oriented Programming Enthusiasts:**
> 
> Python is deeply object-oriented; all elements, including basic data types, are objects.

### Example: Variables and Constants

Create and run the following script:

```python
# Filename : var.py
i = 5
print(i)
i = i + 1
print(i)

s = '''This is a multi-line string.
This is the second line.'''
print(s)
```

Output:

```
5
6
This is a multi-line string.
This is the second line.
```

**How It Works:**

This program assigns the value `5` to `i`, prints it, increments `i`, and prints the updated value. It also demonstrates assigning and printing a multi-line string.

> **Note for Static Language Programmers:**
> 
> In Python, you assign values to variables directly, without declaring types.

## Logical vs. Physical Lines

A _physical line_ is what you see in your code editor, while a _logical line_ is how Python interprets statements.

Python assumes one physical line equals one logical line, but you can use semicolons (`;`) to separate multiple logical lines on one physical line:

```python
i = 5; print(i)
```

For breaking long lines, use a backslash (`\`):

```python
s = 'This is a string. \
This continues the string.'
print(s)
```

Python also allows implicit line joining with parentheses, brackets, or braces.

## Importance of Indentation

Python uses indentation to define blocks of code. All statements in a block must be indented consistently. Incorrect indentation leads to errors.

Example of incorrect indentation:

```python
i = 5
# Incorrect indentation below
 print('Value is', i)
print('I repeat, the value is', i)
```

> **Indentation Best Practice:**
> 
> Use four spaces for indentation. Consistency is crucial for code execution and readability.

> **Note for Static Language Programmers:**
> 
> Python uses indentation for code blocks instead of braces.

## Summary

We’ve covered essential concepts including variables, data types, comments, and more. Mastery of these basics will set a strong foundation for more advanced topics like control flow and custom data types.
