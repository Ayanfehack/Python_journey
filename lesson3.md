# Lesson 03: Numeric Data Types & Augmented Assignment

## 1. Integers and Floats
Python has two main types for numbers:
* **Integers (`int`):** Whole numbers (e.g., `5`, `-42`).
* **Floats (`float`):** Numbers with decimals (e.g., `3.14`, `-2.0`).

### Type Conversion (Casting)
You can switch between types using built-in functions:
* `float(5)` $\rightarrow$ `5.0`
* `int(12.9)` $\rightarrow$ `12` (Note: This **truncates** the decimal, it does not round).
* `int("45")` $\rightarrow$ Converts a string to a number.

---

## 2. Arithmetic Operations
Python supports standard math, but also includes specialized operators:

| Operator | Name | Description | Example |
| :--- | :--- | :--- | :--- |
| `+`, `-`, `*` | Basic Math | Add, Subtract, Multiply | `5 * 2` = `10` |
| `/` | Division | **Always** returns a float | `10 / 2` = `5.0` |
| `//` | Floor Division | Returns the largest whole integer | `56 // 12` = `4` |
| `%` | Modulo | Returns the **remainder** | `56 % 12` = `8` |
| `**` | Exponentiation | Raises to the power of | `2 ** 3` = `8` |



> **Note on Floating Point Math:** Because computers use binary, some fractions (like `0.1 + 0.2`) result in tiny rounding errors (e.g., `0.30000000000000004`). This is a limitation of hardware, not a bug in your code.

---

## 3. Useful Math Functions
* `round(number, ndigits)`: Rounds to the nearest integer or decimal place.
* `abs(number)`: Returns the absolute (positive) value.
* `pow(base, exp, mod)`: Can perform power and modulo in one step (e.g., `(2**3) % 5`).

---

## 4. Augmented Assignment
Instead of writing `x = x + 5`, you can use **Augmented Assignment** to update a variable in place. This is cleaner and prevents typos.

* `+=` (Addition): `price += 10`
* `-=` (Subtraction): `count -= 1`
* `*=` (Multiplication): `total *= 2`
* `/=` (Division): Returns a float.
* `//=` (Floor Division): Returns an int.

### Special Cases with Strings
Some of these operators work with text too!
* `greet += " World"` $\rightarrow$ Concatenates the string.
* `greet *= 3` $\rightarrow$ **Repeats** the string three times.

---

## 5. What Python Doesn't Have
Unlike JavaScript or C#, Python **does not** use `++` or `--`.
* To increment, you must use `x += 1`.
* Writing `++x` in Python won't cause an error, but it **does nothing** (it's just applying a "positive" sign twice).
