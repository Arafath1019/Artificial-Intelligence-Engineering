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