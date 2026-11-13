

# Python Loops & Sequences
-----------

## 1. Lists & Tuples (Sequences)
* **Lists (`list`)**: Ordered, mutable collections supporting zero-based indexing, negative indexing, nested structures, slicing, and unpacking with collection operators (`*rest`).
  * *Common Methods*: `.append()`, `.extend()`, `.insert()`, `.remove()`, `.pop()`, `.clear()`, `.sort()`, `.reverse()`, `.index()`, and the built-in `sorted()`.
* **Tuples (`tuple`)**: Ordered, immutable collections of mixed data types. 
  * *Common Methods*: `.count()`, `.index()`.
  * *Best Practice*: Use lists for dynamic, modifiable collections; use tuples for fixed, immutable data structures.

## 2. Loops & Control Flow
* **`for` Loop**: Iterates sequentially over any iterable (lists, tuples, strings) and supports nesting and `else` completion blocks.
* **`while` Loop**: Executes a block of code repeatedly while a specified condition evaluates to `True`.
* **Loop Control Statements**:
  * `break`: Immediately exits the current loop.
  * `continue`: Skips the current iteration and jumps to the next.
  * `else` Clause: Executes only if the loop finishes completely without hitting a `break` statement.

## 3. Ranges & Iteration Utilities
* **`range(start, stop, step)`**: Generates an immutable sequence of integers. Supports negative steps for decrementing counts and requires integer arguments.
* **`enumerate(iterable, start=0)`**: Returns an iterator yielding pairs of indices and values during iteration.
* **`zip(*iterables)`**: Combines multiple iterables in parallel, iterating through them simultaneously.

## 4. Advanced Iteration: Comprehensions & Functions
* **List Comprehensions**: Concise syntax combining loops and optional conditional filtering/transformations inside square brackets:
  
```python
  even_numbers = [num for num in range(21) if num % 2 == 0]
```
----------



* **Iterable Functions:**

* **`filter(func, iterable):`** Filters elements based on a boolean-returning function.
- **`map(func, iterable):`** Applies a function across all items in an iterable.
- **`sum(iterable, start):`** Computes the total sum of numeric iterables with an optional starting value.

* **`Lambda Functions:`** Anonymous, single-expression functions created using the lambda keyword, ideal for short, one-off operations passed into higher-order functions:


```python
even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
```
