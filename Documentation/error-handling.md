
# Python Error Handling & Debugging 
---------

## 1. Common Python Errors
* **`SyntaxError`**: Raised when code violates Python’s grammar and syntax rules (e.g., unclosed parentheses).
* **`NameError`**: Triggered when accessing an undefined variable or function name.
* **`TypeError`**: Occurs when an operation or function is applied to an object of an inappropriate type (e.g., adding a string to an integer).
* **`IndexError`**: Raised when attempting to access an out-of-bounds index in sequences like lists, tuples, or strings.
* **`AttributeError`**: Triggered when calling a method or property that does not exist on an object type.

## 2. Debugging Techniques
* **Print Debugging**: Strategically placing `print()` statements to track variable states and execution flow.
* **Built-in Debugger (`pdb`)**: Using `pdb.set_trace()` from the standard library to pause execution and open an interactive terminal prompt.
* **IDE Debugging Tools**: Leveraging features in VS Code and PyCharm:
  * **Breakpoints**: Red dots in the editor gutter to pause execution.
  * **Stepping Controls**: Continue (`F5`), Step Over (`F10`), Step Into (`F11`), and Step Out (`Shift + F11`).
  * **Variable Inspection & Debug Console**: Inspecting live variables and evaluating expressions interactively.

## 3. Exception Handling Control Flow
* **`try...except`**: Anticipates and catches runtime errors. Multiple or grouped exceptions can be handled using tuples (e.g., `except (ValueError, ZeroDivisionError) as e:`).
* **`else` & `finally`**: 
  * `else`: Executes only if the `try` block completes successfully with zero exceptions.
  * `finally`: Always executes regardless of whether an exception occurred or was handled.
* **`raise` Statement**: Manually triggers exceptions or re-raises caught exceptions (using plain `raise` inside an `except` block) to propagate them up the call stack.
* **`assert` Statement**: Evaluates debugging assumptions, raising an `AssertionError` if false. *Note: Disabled in optimized mode (`-O`), so never use for critical input validation.*

## 4. Custom Exceptions & Exception Chaining
* **Custom Exceptions**: Created by subclassing the base `Exception` class to implement domain-specific error logic and messages:
  ```python
  class InvalidCredentialsError(Exception):
      pass

* **Exception Chaining (from):**
- `raise NewError() from e:` Preserves the original exception (e) as the underlying cause in the traceback.
- `raise NewError() from None:` Suppresses the original exception context entirely.






  
