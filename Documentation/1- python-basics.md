
# Python Basic:
---------


## 1. Syntax, Variables & Comments
* **Python Overview**: A clean, readable, general-purpose language heavily utilized in data science, automation, web development, and scripting.
* **Variables & Naming**: Dynamically typed (no type declaration needed). Names must start with a letter or underscore, contain alphanumeric characters/underscores, be case-sensitive, avoid reserved keywords, and follow `snake_case` conventions.
* **Comments**: Single-line (`#`) and multi-line comments.
* **`print()`**: Outputs data to the terminal; multiple arguments are separated by spaces by default.

## 2. Common Data Types & Functions
* **Data Types**: Integers (`int`), Floats (`float`), Strings (`str`), and Booleans (`bool`).
* **Type Checking**:
  * `type(var)`: Returns the data type of a variable.
  * `isinstance(val, type)`: Checks if a value matches a specified type (or tuple of types).

## 3. Working with Strings
* **Immutability**: Strings cannot be modified in-place; reassigning variables points them to new values.
* **Indexing & Slicing**: 
  * Access characters via bracket notation (supports negative indexing like `[-1]` from the end).
  * Slice syntax: `str[start:stop:step]` (e.g., `[::-1]` reverses a string).
* **Concatenation & Formatting**: Combine using `+`, `+=`, or compact **f-strings** (`f'Text {expression}'`).
* **String Methods**: `.upper()`, `.lower()`, `.strip()`, `.replace()`, `.split()`, `.join()`, `.startswith()`, `.endswith()`, `.find()`, `.count()`, `.capitalize()`, `.title()`, and translation tables (`str.maketrans()` / `.translate()`).

## 4. Numbers & Math Operations
* **Basic Math**: Addition (`+`), Subtraction (`-`), Multiplication (`*`), Division (`/` returns float).
* **Advanced Operators**: Modulo (`%`), Floor Division (`//`), Exponentiation (`**`), and augmented assignments (`+=`, `-=`, etc.).
* **Math Built-ins**: `float()`, `int()`, `round()`, `abs()`, and `pow()`.

## 5. Functions & Scope
* **Functions**: Reusable blocks defined with `def` taking parameters and returning values (defaults to `None` if no `return` is provided). Supports default arguments.
* **Scope**:
  * **Local Scope**: Variables created inside a function are isolated to that function.
  * **Global Scope**: Variables defined outside functions are accessible globally.

## 6. Control Flow & Boolean Logic
* **Conditionals**: Evaluated using `if`, `elif`, and `else` blocks with strict indentation.
* **Truthy & Falsy Values**: 
  * *Falsy*: `None`, `False`, `0`, `0.0`, `''`.
  * *Truthy*: Non-zero numbers, non-empty strings. `bool()` checks truthiness explicitly.
* **Boolean Operators & Short-Circuiting**:
  * `and`: Returns the first falsy operand or the second if both are truthy.
  * `or`: Returns the first truthy operand or the second if both are falsy.
  * `not`: Inverts a boolean or truthy/falsy evaluation to `True` or `False`.
  * *Short-circuiting*: Python evaluates expressions from left to right and stops as soon as the result is determined.
