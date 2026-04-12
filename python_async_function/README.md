# Python - Asynchronous Programming

## 📌 Project Overview

This project introduces the concept of **asynchronous programming in Python** using `asyncio`.
It focuses on writing efficient, non-blocking code by leveraging **coroutines**, **tasks**, and **event loops**.

The main goal is to understand how to run multiple operations concurrently without using threads.

---

## 🎯 Learning Objectives

By the end of this project, you should be able to explain:

* The syntax and usage of `async` and `await`
* How to execute an asynchronous program using `asyncio`
* How to run multiple coroutines concurrently
* How to create and manage `asyncio` tasks
* How to use the `random` module, specifically `random.uniform`

---

## 🧠 Concepts Covered

### ✔️ Asynchronous Programming

Asynchronous programming allows a program to handle multiple operations at the same time without blocking execution.

---

### ✔️ Coroutines (`async` / `await`)

Coroutines are special functions defined using `async def`.

Example:

```python id="z2h8l9"
import asyncio

async def say_hello():
    await asyncio.sleep(1)
    return "Hello, async world!"
```

---

### ✔️ Running an Async Program

To run an async function, you use `asyncio.run()`:

```python id="k29d1x"
asyncio.run(say_hello())
```

---

### ✔️ Concurrent Execution

You can run multiple coroutines concurrently using:

```python id="q8sjw1"
await asyncio.gather(task1(), task2(), task3())
```

---

### ✔️ Creating Tasks

Tasks allow coroutines to run in the background:

```python id="a3f7kd"
task = asyncio.create_task(say_hello())
await task
```

---

### ✔️ Random Module

The `random.uniform(a, b)` function returns a random floating-point number between `a` and `b`.

Example:

```python id="v5n2m4"
import random

delay = random.uniform(1, 5)
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

```python id="w0s8ad"
"""This module demonstrates asynchronous programming using asyncio."""
```

* Every function and coroutine must include a descriptive docstring:

```python id="u8x1qp"
async def wait_random(max_delay: int) -> float:
    """Waits for a random delay and returns the delay duration."""
```

⚠️ Note:
Docstrings must be clear, complete sentences explaining the purpose.

---

## 📂 Project Structure

```id="e4t9pl"
.
├── 0-basic_async_syntax.py
├── 1-concurrent_coroutines.py
├── 2-measure_runtime.py
├── 3-tasks.py
├── 4-tasks.py
└── README.md
```

---

## 🚀 Execution

Make files executable:

```bash id="m7r2ws"
chmod +x *.py
```

Run a file:

```bash id="b6y3qp"
./0-basic_async_syntax.py
```

---

## 🧪 Code Style

Check code style:

```bash id="n9k4ld"
pycodestyle .
```

---

## 📚 Resources

* Async IO in Python: A Complete Walkthrough
* asyncio - Asynchronous I/O
* Python `random` module

---

## ✨ Author

* Hamsa Alammar
