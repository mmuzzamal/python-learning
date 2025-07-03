# 05 – Conditional Statements in Python

This section covers conditional statements in Python, which let your programs make decisions based on certain conditions.

---

## 1. The `if` Statement

The `if` statement runs a block of code only if the condition is `True`.

```python
x = 10
if x > 5:
    print("x is greater than 5")
```
In this example, Python checks if `x` is greater than 5. Since it is, the message will be printed.

---

## 2. The `if...else` Statement

Use `if...else` to run one block of code if the condition is `True` and another if it is `False`.

```python
x = 3
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```
Here, since `x` is not greater than 5, the code inside the `else` block will run.

---

## 3. The `if...elif...else` Statement

`elif` (else if) lets you check multiple conditions in sequence.

```python
x = 5
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is equal to 5")
else:
    print("x is less than 5")
```
Python checks each condition in order. When it finds one that is `True`, it runs that block and skips the rest.

---

## 4. Nested `if` Statements

You can put one `if` statement inside another to check more complex conditions.

```python
x = 8
if x > 5:
    print("x is greater than 5")
    if x < 10:
        print("x is also less than 10")
```
In this example, both conditions are checked. If `x` is greater than 5, then Python checks if `x` is also less than 10.

---

## 5. Using Logical Operators with Conditions

You can combine conditions using `and`, `or`, and `not`.

```python
x = 7
if x > 5 and x < 10:
    print("x is greater than 5 and less than 10")
```
This statement checks if both conditions are `True` before running the code block.

---

## 6. The `pass` Statement

Use `pass` as a placeholder when you need a statement but do not want any code to run.

```python
x = 4
if x > 10:
    pass  # Do nothing for now
else:
    print("x is not greater than 10")
```
Here, if the condition is not met, nothing happens. Otherwise, the code in the `else` block will run.

---

# Summary

- Conditional statements allow you to control the flow of your Python programs.
- Use `if`, `elif`, and `else` to check different conditions.
- You can nest `if` statements and combine conditions with logical operators.
- Use `pass` when you need a placeholder for future code.

---
