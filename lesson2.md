# Lesson 02: Deep Dive into Strings

## 1. String Basics & Multiline Strings
In Python, single quotes (`'`) and double quotes (`"`) are treated identically. For text spanning multiple lines, use triple quotes (`"""` or `'''`).

* **Handling Quotes:** To include a quote inside a string, either wrap it in the opposite quote type or use the backslash (`\`) escape character.
    * Example: `"It's a sunny day"` or `'It\'s a sunny day'`.

## 2. Indexing and Immutability
Strings are ordered sequences, meaning every character has a specific position (index) starting at **0**.

* **Positive Indexing:** `my_str[0]` is the first character.
* **Negative Indexing:** `my_str[-1]` is the last character.
* **Immutability:** Once a string is created, **it cannot be changed**. You can reassign a variable to a new string, but you cannot modify a specific character in-place.
    * `greeting[0] = 'H'` will throw a `TypeError`.



---

## 3. Concatenation vs. Interpolation
There are two primary ways to combine strings:

* **Concatenation (`+`):** Joins strings together. You must manually convert non-strings using `str()`.
    * Example: `name + " " + str(age)`
* **F-Strings (Interpolation):** The modern, preferred way. Use `f` before the quotes and `{}` to embed variables directly.
    * Example: `f"Hello {name}, you are {age} years old."`

---

## 4. String Slicing
Slicing allows you to extract a specific portion of a string using the syntax `[start:stop:step]`.

* **Non-inclusive:** The `stop` index is not included in the result.
* **Defaults:** Omitting `start` defaults to `0`; omitting `stop` defaults to the end of the string.
* **Reversing:** A common trick to reverse a string is `my_str[::-1]`.

```python
text = "Python"
print(text[0:2])  # "Py"
print(text[2:])   # "thon"
```

---

## 5. Essential String Methods
Methods are built-in functions that run on a string to return a **new** modified version (remember, the original stays the same due to immutability).

| Method | Action |
| :--- | :--- |
| `.upper()` / `.lower()` | Changes casing. |
| `.strip()` | Removes leading/trailing whitespace. |
| `.replace(old, new)` | Swaps parts of the string. |
| `.split()` | Turns a string into a **List**. |
| `.join()` | Turns a List into a **String**. |
| `.startswith()` / `.endswith()` | Returns a Boolean check. |
| `.find()` | Returns the index of a substring (or -1). |

---

### Quiz Reference
* **Extracting portions:** Use square brackets `[]` with start/stop.
* **Outcome of `'Hello'[2:]`:** `llo` (starts at index 2 'l' and goes to the end).
* **Step Parameter:** Defines the increment (e.g., every 2nd character).
* **Case Checking:** Use `isupper()` and `islower()`.

---

### Key Takeaway
Strings are **objects**. Every time you use a method like `.upper()` or perform a slice, Python is creating a **brand new string** in memory because the original cannot be altered.
