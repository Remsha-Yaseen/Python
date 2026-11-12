
# Python Dictionaries, Sets & Standard Library 
-----------

## 1. Dictionaries
* **Definition**: Mutable collections of unique key-value pairs that preserve insertion order. Keys must be hashable (strings, numbers, tuples of hashables).
* **Methods**: `.get()`, `.keys()`, `.values()`, `.items()`, `.pop()`, `.popitem()`, `.update()`, and `.clear()`.
* **Iteration**: Easily loop over keys, values (`.values()`), or key-value pairs (`.items()`), often combined with `enumerate()`.

## 2. Sets & Mathematical Operations
* **Definition**: Mutable, unordered collections of unique, hashable elements. Use `set()` to create an empty set (since `{}` creates a dictionary).
* **Set Methods**: `.add()`, `.remove()` (raises `KeyError` if missing), `.discard()` (safe), and `.clear()`.
* **Set Operators**:
  * **Union (`|` / `|=`)**: Combines elements from both sets.
  * **Intersection (`&` / `&=`)**: Keeps only shared elements.
  * **Difference (`-` / `-=`)**: Elements in the first set but not the second.
  * **Symmetric Difference (`^` / `^=`)**: Elements in either set, but not both.
  * **Relational Methods**: `.issubset()`, `.issuperset()`, and `.isdisjoint()`.

## 3. Python Standard Library & Imports
* **Standard Library**: Pre-built modules like `math`, `random`, `re`, and `datetime`.
* **Import Variations**:
  * `import module_name` (access via dot notation).
  * `import module_name as alias` (aliasing).
  * `from module_name import name1, name2` (import specific items).
  * `from module_name import *` (wildcard import — generally discouraged due to namespace pollution).
* **Execution Guard (`if __name__ == '__main__'`)**: Checks whether a script is run directly (`'__main__'`) versus being imported as a module.

## 4. Data Validation & Regular Expressions (`re`)
* **Dictionary Unpacking (`**`)**: Unpacks a dictionary into keyword arguments.
* **Regular Expressions (`re`)**:
  * `re.search(pattern, string)`: Finds the first occurrence of a pattern (returns a match object or `None`).
  * `re.fullmatch(pattern, string)`: Matches the entire string.
  * `re.IGNORECASE`: Flag for case-insensitive matching.
  * **Raw Strings (`r''`) & Quantifiers**: Treats backslashes literally (`r'\d'` matches digits; `+` matches one or more repetitions).
* **Utilities**: Object identity checks (`is` / `is not`, standard for checking `None`) and `all()` (returns `True` if every element in an iterable is truthy).

---

### Placement Recommendation
* **Target Section**: **`🔹 Module 1: Python Fundamentals`** (or advanced Python data structures section)
* **Suggested Entry**: 
  ```markdown
  * [dictionaries-sets-and-modules.md](./dictionaries-sets-and-modules.md) — Comprehensive guide on Python dictionaries, sets, module imports, `__name__ == '__main__'`, data validation, and regular expressions.
