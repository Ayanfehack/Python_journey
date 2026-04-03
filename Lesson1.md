# Lesson 01: Python Fundamentals - Variables, Output, and Data Types

## 1. Variables & Assignment
In Python, variables act as labeled boxes for storing data. Unlike languages like C# or Java, Python does not require special keywords (like `let` or `int`) to declare them.

* **Assignment Operator:** Use the `=` symbol to assign a value to a variable name.
* **Dynamic Typing:** Python automatically determines the data type based on the value assigned.

```python
name = 'John Doe'  # Python identifies this as a string
age = 25           # Python identifies this as an integer
```

### Naming Rules (Avoid Syntax Errors)
1. Must start with a **letter** or **underscore** (`_`), never a number.
2. Can only contain letters, numbers, and underscores.
3. **Case-sensitive:** `age`, `Age`, and `AGE` are three different variables.
4. Cannot use **reserved keywords** (e.g., `if`, `class`, `def`).

### Naming Conventions
* **Snake Case:** Use lowercase with underscores for multi-word variables (e.g., `user_age`).
* **Descriptive Names:** Use `total_price` instead of `tp`. Avoid single-letter names unless used in loops (like `i`).

---

## 2. Comments
Comments are used to explain code or leave reminders. Python ignores everything following the `#` symbol.

```python
# This is a single-line comment
# This is a
# multi-line comment
```

---

## 3. The `print()` Function
The `print()` function outputs data to the terminal. You can pass multiple **arguments** separated by commas, and Python will automatically add a space between them.

```python
print('Hello world!')
print('My favorite colors are', 'blue', 'green') 
# Output: My favorite colors are blue green
```

---

## 4. Data Types
Understanding data types is crucial because they define how the computer handles information.

### Common Python Data Types
| Type | Description | Example |
| :--- | :--- | :--- |
| **Integer (`int`)** | Whole numbers | `10`, `-5` |
| **Float (`float`)** | Decimal numbers | `4.5`, `-0.4` |
| **String (`str`)** | Text in single/double quotes | `'hello'`, `"world"` |
| **Boolean (`bool`)** | Logical values | `True`, `False` |
| **List (`list`)** | Ordered collection (mutable) | `[1, 'a', 3.14]` |
| **Tuple (`tuple`)** | Ordered collection (immutable) | `(1, 2, 3)` |
| **Dictionary (`dict`)**| Key-value pairs | `{'name': 'Alice'}` |
| **Set (`set`)** | Unique unordered elements | `{1, 2, 3}` |
| **NoneType** | Represents the absence of a value | `None` |



---

## 5. Type Checking
Since Python is **dynamically typed**, errors are caught during **runtime** (execution) rather than during a compile step. Use these functions to verify types:

* **`type()`**: Returns the data type of a variable.
* **`isinstance()`**: Checks if a variable belongs to a specific type (returns `True`/`False`).

```python
my_var = "Hello"
print(type(my_var))              # <class 'str'>
print(isinstance(my_var, str))   # True
```
