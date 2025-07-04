# 06 – Control Flow in Python

Control flow statements determine the order in which code executes in a Python program. They help you repeat actions (loops) or exit them based on conditions.

---

## 1. The `while` Loop

A `while` loop repeats a block of code as long as a condition is `True`.

```python
count = 1
while count <= 3:
    print(count)
    count += 1
```
This loop prints the numbers 1, 2, and 3. The loop continues as long as `count` is less than or equal to 3.

---

## 2. The `for` Loop

A `for` loop iterates over a sequence (like a list, tuple, or string).

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```
This loop prints each fruit in the list, one at a time.

---

## 3. The `range()` Function

`range()` generates a sequence of numbers, which is often used with `for` loops.

```python
for i in range(3):
    print(i)
```
This prints 0, 1, and 2. The loop runs three times, starting from 0 up to (but not including) 3.

---

## 4. The `break` Statement

Use `break` to exit a loop early when a condition is met.

```python
for number in range(1, 10):
    if number == 5:
        break
    print(number)
```
This loop prints 1 to 4. When `number` reaches 5, the loop stops.

---

## 5. The `continue` Statement

Use `continue` to skip the rest of the current loop iteration and move to the next one.

```python
for number in range(1, 6):
    if number == 3:
        continue
    print(number)
```
This prints 1, 2, 4, and 5. When `number` is 3, the `print()` statement is skipped.

---

## 6. The `else` Clause with Loops

An `else` block after a loop runs when the loop finishes normally (not when it's ended by `break`).

```python
for i in range(3):
    print(i)
else:
    print("Loop finished!")
```
This prints 0, 1, 2, and then "Loop finished!" after the loop ends.

---

## 7. Nested Loops

You can place one loop inside another to work with multiple sequences.

```python
for i in range(1, 3):
    for j in range(1, 3):
        print(f"i={i}, j={j}")
```
This prints all combinations of `i` and `j` from 1 to 2.

---

# Summary

- Control flow statements (`while`, `for`, `break`, `continue`, `else` with loops) control how and when code runs.
- Loops help repeat actions efficiently.
- Use `break` and `continue` to control loop behavior.
- Use nested loops to handle more complex tasks.

---
