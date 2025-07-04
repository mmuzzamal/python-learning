# 09 – Data Structures in Python

Data structures are special ways to organize and store information in your programs. Think of them as different types of containers, each designed for a specific kind of job—just like you use a wallet for money, a jar for cookies, and a filing cabinet for documents.

This section covers:
- What data structures are
- The four most common ones in Python (List, Tuple, Set, Dictionary)
- Real-world examples and use cases for each
- How to decide which one to use
- Nested (combined) data structures

---

## 1. What Are Data Structures?

Imagine you’re organizing your home:

- A **list** is like a shopping list—you can add, remove, or rearrange items any time.
- A **tuple** is like a sealed box of medals—you know what’s inside, but you can’t change them.
- A **set** is like a guest list for a party—no one is invited twice, and the order does not matter.
- A **dictionary** is like a contact book, where you look up people (keys) to get their phone numbers (values).

**Why do we use data structures?**
- To keep our data organized and easy to access.
- To make our programs faster and easier to write.
- To solve real-world problems in a logical way.

---

## 2. List

A **list** is an ordered collection that you can change (add, remove, or update items). It can hold any type of data: numbers, words, or even other lists.

### Real-world example:
**Shopping List:**  
You keep adding or removing items before going to the store.

```python
shopping_list = ["bread", "milk", "eggs"]
print(shopping_list[1])   # milk

# Add an item
shopping_list.append("butter")
print(shopping_list)      # ["bread", "milk", "eggs", "butter"]

# Remove an item
shopping_list.remove("bread")
print(shopping_list)      # ["milk", "eggs", "butter"]

# Change an item
shopping_list[0] = "almond milk"
print(shopping_list)      # ["almond milk", "eggs", "butter"]
```

**Use case:**  
Any situation where the order matters and you may need to change the data later—like managing tasks, scores, or a playlist.

---

## 3. Tuple

A **tuple** is also an ordered collection, but you **cannot change** it after it’s created. It’s like writing something in permanent ink.

### Real-world example:
**Storing GPS coordinates:**  
A latitude and longitude should never be changed accidentally.

```python
location = (31.5204, 74.3587)  # (latitude, longitude)

print(location[0])  # 31.5204

# Trying to change a tuple will result in an error
# location[0] = 0  # This will cause an error!
```

**Use case:**  
When you want to make sure your data stays constant, like days of the week, RGB color codes, or database records.

---

## 4. Set

A **set** is an unordered collection of unique items. Think of it as a basket where each fruit appears only once, no matter how many times you add it.

### Real-world example:
**Keeping track of unique visitors to your website:**  
You do not want to count the same person twice.

```python
unique_visitors = {"Ali", "Sara", "Ali", "John"}
print(unique_visitors)  # {"Ali", "Sara", "John"} (order may vary)

# Add a new visitor
unique_visitors.add("Fatima")
print(unique_visitors)

# Check if someone visited
print("Sara" in unique_visitors)  # True
```

**Use case:**  
Any scenario where you need to remove duplicates or check if something exists, like tags, unique IDs, or participants in an event.

---

## 5. Dictionary

A **dictionary** stores data as key-value pairs. It’s like a real dictionary: you look up a word (key) to find its meaning (value).

### Real-world example:
**Contact information:**  
You look up a name to get a phone number.

```python
contacts = {
    "Ali": "03001234567",
    "Sara": "03211234567",
    "John": "03111234567"
}

print(contacts["Sara"])  # 03211234567

# Add a new contact
contacts["Fatima"] = "03451234567"
print(contacts)

# Update a contact
contacts["Ali"] = "03007654321"
print(contacts)

# Remove a contact
del contacts["John"]
print(contacts)
```

**Use case:**  
When you need to map one thing to another, like student roll numbers to names, country codes to country names, or usernames to passwords.

---

## 6. When to Use Which Data Structure?

Choosing the right data structure depends on your problem.

| Data Structure | Use When…                                            | Example                                   |
| -------------- | ---------------------------------------------------- | ----------------------------------------- |
| List           | You need order, can have duplicates, and may update  | Shopping list, playlist, queue            |
| Tuple          | Order matters, but data should never change          | GPS coordinates, RGB color, days of week  |
| Set            | Uniqueness matters, order does not, fast lookup      | Unique visitors, tags, unique IDs         |
| Dictionary     | You want to pair keys with values, fast lookup       | Contacts, marksheet, product catalog      |

### **Some quick comparisons:**

- **List vs Tuple:**  
  Use a tuple if you do not want anyone to accidentally change the data.

- **List vs Set:**  
  Use a set if you only care about unique items and do not care about their order.

- **Dictionary vs List of Tuples:**  
  Use a dictionary if you need to look things up by a unique key.  
  Use a list of tuples if you want to keep pairs but do not need fast lookup.

---

## 7. Nested Data Structures

You can combine data structures to solve more complex problems—just like putting boxes inside other boxes.

### Real-world examples:

- **Classroom record:** Each student has a name and a list of marks.

```python
students = [
    {"name": "Ali", "marks": [85, 90, 88]},
    {"name": "Sara", "marks": [92, 81, 77]},
    {"name": "John", "marks": [78, 85, 80]}
]
print(students[1]["marks"][2])  # 77
```

- **Phonebook with multiple numbers per person:**

```python
phonebook = {
    "Ali": ["03001234567", "03007654321"],
    "Sara": ["03211234567"],
    "John": []
}
print(phonebook["Ali"][1])  # 03007654321
```

- **Chess board (list of lists):**

```python
board = [
    ["R", "N", "B", "Q", "K", "B", "N", "R"],  # Row 1
    ["P", "P", "P", "P", "P", "P", "P", "P"],  # Row 2
    ["", "", "", "", "", "", "", ""],           # Row 3
    # ... more rows ...
]
print(board[0][3])  # Q
```

---

## 8. Summary

- Data structures help organize and manage data efficiently.
- Lists, tuples, sets, and dictionaries are the most common built-in types in Python.
- Use real-world problems to decide which one fits best.
- You can combine them (nesting) for more complex situations.

---
