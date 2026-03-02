# Full Stack Generative and Agentic AI with Python

## 01. Introduction

### 1. Installation of Tools (VSCode and Python)

* Download & Install VSCode as IDE: https://code.visualstudio.com/
* Download & Install Python: https://www.python.org/

## 02. Introduction to Coding world with Python

### 2. What is Programming

* https://code.visualstudio.com/
* https://www.eraser.io/
* https://www.tldraw.com/
* https://excalidraw.com/

### 4. A Real World Python Code
```
class Chai:
    def __init__(self, sweetness, milk_level):
        self.sweetness = sweetness
        self.milk_level = milk_level
    
    def sip(self):
        print("Sipping chai")
    
    def add_sugar(self, amount):
        print("Added the sugar")

my_chai = Chai(sweetness=3, milk_level=2)

my_chai.add_sugar(3)
```

### 5. Why to use Python

- Portable (Windows, mac, linux)
- Readable
- Productive
- Standard library
- Multi-use

### 6. Writing first Python code on Mac

- Download & install python: https://www.python.org/
- Warp Terminal: https://www.warp.dev/

### 8. Get Everything in Virtual Environment
A Python virtual environment is an isolated Python runtime + package directory for a project so each project can have its own dependencies and versions without affecting the system Python or other projects.

- Why use it: avoids dependency conflicts, improves reproducibility, and keeps global environment clean.
- Create (built-in):
```
python -m venv env
```
- Activate (macOS/Linux):
```
source env/bin/activate
```
- Install deps / freeze:
```
pip install -r requirements.txt
pip freeze > requirements.txt
```
- Deactivate:
```
deactivate
```

- Alternatives / tooling: uv, virtualenv, pipenv, poetry, and conda (for package + env management).

### 10. PEP8 and Zen of Python

- PEP 8 – Style Guide for Python Code: https://peps.python.org/pep-0008/
- The Zen of Python: https://peps.python.org/pep-0020/
```
Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

## 03. Data Types in Python
#### 1. Objects - Mutable and Immutable in Python
In Python, objects are classified as either mutable or immutable based on whether their state can be changed after creation.

Immutable Objects
Definition: Objects whose value cannot be changed after they are created.
Examples: int, float, complex, bool, str (strings), tuple, frozenset, bytes

Key Characteristics:
- Any modification creates a new object in memory
- More memory-efficient for fixed values
- Hashable (can be used as dictionary keys)
- Thread-safe by nature

Example:
```
# Strings are immutable
name = "Python"
# name[0] = "J"  # ❌ This would raise an error!

# Modification creates a new object
new_name = name.upper()
print(name)      # "Python" (original unchanged)
print(new_name)  # "PYTHON" (new object)

# Integers are immutable
x = 10
print(id(x))  # Some memory address
x += 5        # This creates a new integer
print(id(x))  # Different memory address
```

Mutable Objects
Definition: Objects whose value can be changed after they are created.
Examples: list, dict, set, Custom class instances, bytearray

Key Characteristics:
- Can be modified in-place
- Changes reflect across all references to the object
- Not hashable (generally)
- More memory-efficient for dynamic data

Example:
```
# Lists are mutable
fruits = ["apple", "banana"]
print(id(fruits))  # Memory address

fruits.append("orange")  # Modify in-place
print(id(fruits))  # Same memory address
print(fruits)      # ["apple", "banana", "orange"]

# Dictionaries are mutable
person = {"name": "Alice", "age": 30}
person["age"] = 31  # Modify in-place
person["city"] = "New York"  # Add new key
print(person)  # {"name": "Alice", "age": 31, "city": "New York"}ß
```