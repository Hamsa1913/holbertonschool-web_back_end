# Python - Asynchronous Generators & Comprehensions

## 📌 Project Overview

This project explores advanced concepts in **asynchronous programming in Python**, focusing on **asynchronous generators** and **asynchronous comprehensions**.

It also emphasizes writing clean, type-safe code using **type annotations**, while maintaining proper documentation and coding standards.

---

## 🎯 Learning Objectives

By the end of this project, you should be able to explain:

* How to write an **asynchronous generator**
* How to use **async comprehensions**
* How to apply **type annotations** to generators and coroutines

---

## 🧠 Concepts Covered

### ✔️ Asynchronous Generators

Asynchronous generators are defined using `async def` and `yield`.
They allow you to produce values asynchronously.

Example:

```python id="g7k2m1"
import asyncio
import random

async def async_generator():
    """Yields random numbers asynchronously."""
    for _ in range(5):
        await asyncio.sleep(1)
        yield random.uniform(0, 10)
```

---

### ✔️ Async Comprehensions

Async comprehensions allow you to iterate over asynchronous iterables using a concise syntax.

Example:

```python id="n3p8q4"
result = [i async for i in async_generator()]
```

---

### ✔️ Type Annotations for Generators

Generators and async generators can be type-annotated for better readability and reliability.

Example:

```python id="x9v2l6"
from typing import AsyncGenerator

async def async_generator() -> AsyncGenerator[float, None]:
    """Returns an async generator of floats."""
```

---

## ⚙️ Requirements

* OS: Ubuntu 20.04 LTS
* Python version: 3.9
* Allowed editors: `vi`, `vim`, `emacs`
* Code style: **pycodestyle (v2.5.x)**

### 📌 File Requirements

* All files must:

  * Start with:

    ```python
    #!/usr/bin/env python3
    ```
  * End with a new line
  * Be executable
  * Pass `wc` length checks

---

## 📝 Documentation Requirements

* Every module must include a meaningful docstring:

```python id="u1w8ex"
"""This module demonstrates asynchronous generators and comprehensions."""
```

* Every function and coroutine must include a descriptive docstring:

```python id="c5r9mz"
async def async_generator() -> AsyncGenerator[float, None]:
    """Generates random float values asynchronously."""
```

⚠️ Note:
Docstrings must be clear, full sentences explaining the purpose.

---

## 📂 Project Structure

```id="h2k7ds"
.
├── 0-async_generator.py
├── 1-async_comprehension.py
├── 2-measure_runtime.py
└── README.md
```

---

## 🚀 Execution

Make files executable:

```bash id="b8p4xy"
chmod +x *.py
```

Run a file:

```bash id="z3n6qa"
./0-async_generator.py
```

---

## 🧪 Code Style

Check code style:

```bash id="d7m1lk"
pycodestyle .
```

---

## 📚 Resources

* PEP 530 -- Asynchronous Comprehensions
* What’s New in Python: Asynchronous Comprehensions / Generators
* Type hints for generators

---

## ✨ Author

* Hamsa Bnian Alammar
