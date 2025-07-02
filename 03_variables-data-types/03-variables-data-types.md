# 03 – Variables and Data Types in Python

This document introduces Python variables and the most common built-in data types, including basic examples of collections.

---

## 1. Simple Variable Assignment

Variables are used to store information in Python.

```python
name = "Muzzamal"
age = 20
country = "Pakistan"

print("Name:", name)
print("Age:", age)
print("Country:", country)
```

---

## 2. Type Checking

You can use the `type()` function to check the data type of any variable.

```python
num = 5
pi = 3.14
greeting = "Hello"
is_coding = True

print("Type of num:", type(num))
print("Type of pi:", type(pi))
print("Type of greeting:", type(greeting))
print("Type of is_coding:", type(is_coding))
```

---

## 3. Swapping Variables

Python allows you to swap variable values easily.

```python
a = 10
b = 20
a, b = b, a
print("After swapping: a =", a, ", b =", b)
```

---

## 4. String Formatting

F-strings let you create readable output with variable values.

```python
first_name = "Muhammad"
last_name = "Muzzamal"
print(f"Hello, my name is {first_name} {last_name}.")
```

---

## 5. Arithmetic Operations

Python can do basic math operations.

```python
num1 = 8
num2 = 3
print("Addition:", num1 + num2)
print("Subtraction:", num1 - num2)
print("Multiplication:", num1 * num2)
print("Division:", num1 / num2)
```

---

## 6. Data Type Conversion

You can convert between compatible types.

```python
int_value = 100
str_value = str(int_value)
print("Integer to string:", str_value, type(str_value))

string_num = "123"
converted_num = int(string_num)
print("String to integer:", converted_num, type(converted_num))
```

**If you try to convert something not compatible, Python will give an error:**
```python
# invalid_conversion = int("hello")  # This will cause a ValueError
```

---

## 7. Boolean Practice

Boolean values represent `True` or `False`.

```python
is_python_fun = True
print("Is Python fun?", is_python_fun)
```

---

## 8. Multiple Assignment

You can assign values to several variables at once.

```python
x, y, z = 1, 2, 3
print("x =", x, "y =", y, "z =", z)
```

---

## 9. User Input

The `input()` function gets input from the user as a string.

```python
favorite_color = input("What is your favorite color? ")
print("Your favorite color is", favorite_color)
```

---

# Basic Collection Types in Python

Python provides several ways to store groups of data.

---

## List

Ordered collection of items, written in square brackets.

```python
fruits = ["apple", "banana", "cherry"]
```

---

## Tuple

Ordered, unchangeable collection, written in parentheses.

```python
point = (3, 4)
```

---

## Dictionary

Unordered collection of key-value pairs, written in curly braces.

```python
person = {"name": "Alice", "age": 25}
```

---

## Set

Unordered collection of unique items, written in curly braces.

```python
unique_numbers = {1, 2, 3}
```

---

# Summary

- Python has several basic data types, including numbers, strings, booleans, and collections.
- You can check a variable’s type with `type()`.
- Lists, tuples, dictionaries, and sets are ways to store multiple items in a single variable.

---
