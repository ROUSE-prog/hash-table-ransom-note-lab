# Hash Tables – Ransom Note Lab

## Overview

This project demonstrates how to solve the classic **Ransom Note** problem using a **hash table (Python dictionary)**. The goal is to determine whether a ransom note can be constructed using the characters from a magazine, where each character may only be used once.

This lab reinforces the use of hash tables for efficient frequency counting and constant-time lookups.

---

## Features

* Implements the `can_construct()` function
* Uses a Python dictionary (hash table) to count character frequencies
* Decrements counts as characters are used
* Returns early when a required character is unavailable
* Handles repeated characters and longer input strings
* Passes all provided unit tests

---

## Project Structure

```
.
├── ransom_note.py          # Solution implementation
├── test_ransom_note.py     # Unit tests
└── README.md               # Project documentation
```

---

## How It Works

1. Count every character in the `magazine` string using a dictionary.
2. Iterate through each character in the `ransomNote`.
3. If a character is unavailable or has already been used, return `False`.
4. Otherwise, decrement its count.
5. Return `True` after successfully matching every character.

This approach runs in **O(n + m)** time, where:

* **n** = length of the magazine
* **m** = length of the ransom note

The algorithm uses **O(n)** additional space for the hash table.

---

## Example

```python
from ransom_note import can_construct

print(can_construct("aa", "aab"))
# True

print(can_construct("aa", "ab"))
# False
```

---

## Running the Tests

Execute the test suite with:

```bash
python test_ransom_note.py
```

If everything is working correctly, all tests will pass successfully.

---

## Technologies Used

* Python 3
* Dictionaries (Hash Tables)
* Unit Testing

---

## Concepts Practiced

* Hash Tables
* Dictionaries
* Frequency Counting
* Conditional Logic
* Algorithm Design
* Time and Space Complexity Analysis

