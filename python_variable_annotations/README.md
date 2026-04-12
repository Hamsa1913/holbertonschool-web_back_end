# Python - Type Annotations

## 📌 Project Overview

This project focuses on understanding and applying **type annotations in Python 3**.
It covers how to write clean, well-documented, and type-safe Python code using modern best practices.

The goal is to improve code readability, maintainability, and reliability by leveraging Python's typing system.

---

## 🎯 Learning Objectives

By the end of this project, you should be able to explain:

* What **type annotations** are in Python 3
* How to use type hints to define:

  * Function parameters
  * Return types
  * Variables
* The concept of **duck typing**
* How to validate your code using **mypy**
* The importance of writing clean and documented code

---

## 🧠 Concepts Covered

### ✔️ Type Annotations

Type annotations allow you to specify expected data types for variables, function arguments, and return values.

Example:

```python
def add(a: int, b: int) -> int:
    return a + b
```

---

### ✔️ Duck Typing

Python follows duck typing:

> "If it looks like a duck and quacks like a duck, it's a duck."

This means Python focuses on behavior rather than explicit types.

---

### ✔️ Static Type Checking with mypy

`mypy` is a tool used to check type correctness before runtime.

Run:

```bash
mypy your_file.py
```

---

## ⚙️ Requirements

* OS: Ubuntu 20.04 LTS
* Python version: 3.9
* Allowed editors: `vi`, `vim`, `emacs`
* Code style: **pycodestyle (v2.5)**
* All files must:

  * End with a new line
  * Start with:

    ```python
    #!/usr/bin/env python3
    ```
  * Be executable
  * Pass `wc` length checks

---

## 📂 Project Structure

```
.
├── 0-add.py
├── 1-concat.py
├── 2-floor.py
├── 3-to_str.py
├── ...
└── README.md
```

---

## 📝 Documentation Requirements

* Every module must include a meaningful docstring:

```python
"""This module provides basic arithmetic operations using type annotations."""
```

* Every class must include a docstring
* Every function must include a descriptive docstring:

```python
def add(a: int, b: int) -> int:
    """Returns the sum of two integers."""
```

⚠️ Note:
Docstrings must be full sentences explaining the purpose — not just one word.

---

## 🚀 Execution

Make files executable:

```bash
chmod +x *.py
```

Run a file:

```bash
./0-add.py
```

---

## 🧪 Code Style

Check style:

```bash
pycodestyle .
```

---

## 📚 Resources

* Python 3 typing documentation
* MyPy cheat sheet

---

## ✨ Author

* Hamsa Bnian Alammar
