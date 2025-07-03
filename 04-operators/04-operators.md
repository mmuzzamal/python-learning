# 04 – Operators in Python

This section introduces the main types of operators in Python, with simple examples for each.

---

## 1. Arithmetic Operators

Used for mathematical operations.

```python
a = 10
b = 3

print(f"Addition: {a + b}")         # 13
print(f"Subtraction: {a - b}")      # 7
print(f"Multiplication: {a * b}")   # 30
print(f"Division: {a / b}")         # 3.333...
print(f"Floor Division: {a // b}")  # 3
print(f"Modulus: {a % b}")          # 1
print(f"Exponent: {a ** b}")        # 1000
```

---

## 2. Assignment Operators

Used to assign values to variables.

```python
x = 5      # Assigns 5 to x
x += 2     # x = x + 2 → 7
x -= 3     # x = x - 3 → 4
x *= 2     # x = x * 2 → 8
x /= 4     # x = x / 4 → 2.0
x //= 2    # x = x // 2 → 1.0
x %= 2     # x = x % 2 → 1.0
x **= 3    # x = x ** 3 → 1.0
print(f"Final x: {x}")
```

---

## 3. Comparison Operators

Used to compare two values. The result is always `True` or `False`.

```python
a = 7
b = 5

print(f"Equal: {a == b}")               # False
print(f"Not Equal: {a != b}")           # True
print(f"Greater Than: {a > b}")         # True
print(f"Less Than: {a < b}")            # False
print(f"Greater or Equal: {a >= b}")    # True
print(f"Less or Equal: {a <= b}")       # False
```

---

## 4. Logical Operators

Used to combine conditional statements.

```python
is_sunny = True
is_warm = False

print(f"AND: {is_sunny and is_warm}")     # False
print(f"OR: {is_sunny or is_warm}")       # True
print(f"NOT: {not is_sunny}")             # False
```

---

## 5. Identity Operators

Used to compare the memory location of two objects.

```python
x = [1, 2, 3]
y = [1, 2, 3]
z = x

print(f"x is z: {x is z}")           # True (same object)
print(f"x is y: {x is y}")           # False (different objects with same content)
print(f"x is not y: {x is not y}")   # True
```

---

## 6. Membership Operators

Used to test if a value is present in a sequence (list, tuple, string, etc.).

```python
fruits = ["apple", "banana", "cherry"]

print(f"banana in fruits: {'banana' in fruits}")          # True
print(f"orange in fruits: {'orange' in fruits}")          # False
print(f"grape not in fruits: {'grape' not in fruits}")    # True
```

---

# Summary

- Python operators are symbols that perform operations on variables and values.
- There are arithmetic, assignment, comparison, logical, identity, and membership operators.
- Operators help you write concise and readable code for everyday programming tasks.

---
