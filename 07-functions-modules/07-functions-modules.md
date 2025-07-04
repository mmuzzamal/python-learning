# 07 – Functions and Modules in Python

In this section, you'll learn how to create reusable blocks of code using functions, and how to organize your code using modules.

---

## 1. What is a Function?

A function is a named block of code that performs a specific task. Functions help you organize, reuse, and simplify your code.

---

### Defining and Calling a Function

Use the `def` keyword to define a function. Call (run) the function by writing its name followed by parentheses.

```python
def greet():
    print("Hello, welcome to Python!")

greet()  # Calls the function
```
This defines a function called `greet` and then calls it, printing a message.

---

## 2. Function Parameters and Arguments

Functions can accept information (parameters) so they can work with different data.

```python
def add(a, b):
    print(a + b)

add(3, 5)  # Outputs: 8
```
Here, `a` and `b` are parameters. When you call `add(3, 5)`, `3` and `5` are arguments passed to the function.

---

## 3. Return Values

Functions can return a value using the `return` statement.

```python
def multiply(a, b):
    return a * b

result = multiply(4, 6)
print(result)  # Outputs: 24
```
This function returns the product of `a` and `b`, which is then printed.

---

## 4. Default Parameter Values

You can give parameters default values. If an argument isn’t provided, the default is used.

```python
def greet(name="friend"):
    print("Hello,", name)

greet()          # Outputs: Hello, friend
greet("Sara")    # Outputs: Hello, Sara
```
Here, `name` defaults to `"friend"` if no argument is given.

---

## 5. Keyword Arguments

You can specify arguments by name when calling a function.

```python
def introduce(name, age):
    print("My name is", name, "and I am", age, "years old.")

introduce(age=25, name="Ali")
```
This lets you pass arguments in any order.

---

## 6. What is a Module?

A module is a file containing Python code (functions, variables, etc.) that you can use in other programs. Modules help organize code into separate files.

---

### Importing Modules

Use the `import` statement to bring in a module.

```python
import math

print(math.sqrt(16))  # Outputs: 4.0
```
This imports Python’s built-in `math` module and uses its `sqrt()` function.

---

### Importing Specific Parts of a Module

You can import only what you need from a module.

```python
from math import pi

print(pi)  # Outputs: 3.141592653589793
```
This imports just the `pi` variable from the `math` module.

---

## 7. Creating and Using Your Own Module

You can create your own module by saving functions in a `.py` file, then importing it.

Suppose you have a file called `my_utils.py`:

```python
# my_utils.py
def say_hi():
    print("Hi from my_utils!")
```

You can import and use it in another file:

```python
import my_utils

my_utils.say_hi()
```
This calls the `say_hi()` function from your custom module.

---

# Summary

- Functions help you organize and reuse code.
- Functions can accept parameters, return values, and have default values.
- Modules let you organize code into multiple files.
- Use `import` to access functions and variables from modules.

---
