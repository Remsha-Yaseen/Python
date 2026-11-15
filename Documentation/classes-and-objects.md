
# Python Classes & Objects
-----


## 1. Classes, Instantiation & Attributes
* **Class Definition**: A blueprint for creating objects using PascalCase naming conventions (e.g., `Dog`, `ShoppingCart`).
* **Initialization (`__init__`) & `self`**: 
  * `__init__()` automatically executes upon object creation to set initial attributes.
  * `self` refers to the specific instance being operated on and is always the first parameter of instance methods.
* **Instance vs. Class Attributes**:
  * *Instance Attributes*: Unique to each object, typically defined inside `__init__()` via `self`.
  * *Class Attributes*: Defined directly inside the class body and shared across all instances.
* **Dynamic Attribute Handling & Inspection**:
  * Built-in functions: `getattr(obj, name, default)`, `setattr(obj, name, value)`, `hasattr(obj, name)`, and `delattr(obj, name)`.
  * `dir(obj)` returns a list of all attributes and methods, which can be filtered using `callable()` to distinguish data attributes from methods.

## 2. Methods & Dunder (Magic) Methods
* **Instance Methods**: Functions defined inside a class that interact with object attributes via dot notation (`object.method()`).
* **Dunder Methods**: Special double-underscore methods (`__init__`, `__str__`, `__eq__`, `__len__`, `__getitem__`, `__contains__`, `__iter__`) that empower custom objects to integrate seamlessly with Python's built-in operations and operators.

## 3. Object Collaboration & Composition
* **Composition**: Objects can be passed as arguments to other constructors or stored as attributes inside other objects (e.g., a `User` containing an `Inbox` object holding `Email` objects), enabling complex data modeling through dot-notation chaining (`receiver.inbox.emails[0].body`).

## 4. Working with Dates and Times (`datetime`)
* **Timestamps**: Generating creation timestamps using `datetime.datetime.now()` assigned to instance attributes.
* **Formatting (`strftime`)**: Converting `datetime` objects into readable strings using format directives (e.g., `%Y-%m-%d %H:%M:%S` for year, month, day, hour, minute, second).
