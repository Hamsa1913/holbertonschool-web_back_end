# Python - Asynchronous Programming (Full Repository)

## 📌 Overview

This repository contains a series of projects that cover **asynchronous programming in Python** from fundamentals to advanced concepts.

The projects are designed to build a solid understanding of how Python handles concurrency using `asyncio`, including:

* Basic asynchronous execution
* Managing coroutines and tasks
* Asynchronous generators
* Async comprehensions
* Type annotations in async code

---

## 🎯 Objectives

By completing this repository, you will be able to:

* Understand and use `async` and `await`
* Execute asynchronous programs using `asyncio`
* Run multiple coroutines concurrently
* Create and manage tasks with `asyncio`
* Write asynchronous generators
* Use async comprehensions effectively
* Apply type annotations to functions and coroutines
* Write clean, well-documented Python code

---

## 🧠 Topics Covered

### ✔️ Asynchronous Execution

Understanding non-blocking execution and how Python manages tasks efficiently using an event loop.

---

### ✔️ Coroutines & Tasks

* Defining coroutines with `async def`
* Using `await` to pause execution
* Running concurrent tasks using:

```python
await asyncio.gather(...)
```

---

### ✔️ Asynchronous Generators

Creating generators that yield values asynchronously using `async def` and `yield`.

---

### ✔️ Async Comprehensions

Using concise syntax to iterate over async iterables:

```python
[i async for i in async_generator()]
```

---

### ✔️ Type Annotations

Applying type hints for better readability and maintainability, including:

* Function parameters
* Return types
* Async generators (`AsyncGenerator`)

---

## 📂 Repository Structure

```id="k8f2mz"
.
├── 0x00-python_async_function/
├── 0x01-python_async_comprehension/
├── 0x02-python_async_generators/
└── README.md
```

---

## ⚙️ Requirements

* OS: Ubuntu 20.04 LTS
* Python version: 3.9
* Allowed editors: `vi`, `vim`, `emacs`
* Code style: **pycodestyle (v2.5.x)**

### 📌 File Rules

* All files must:

  * Start with:

    ```python
    #!/usr/bin/env python3
    ```
  * End with a new line
  * Be executable
  * Pass `wc` checks

---

## 📝 Documentation Standards

* Each module must include a meaningful docstring
* Each function/coroutine must include a clear docstring
* Documentation must be:

  * Descriptive
  * Written in full sentences
  * Explaining the purpose of the code

Example:

```python
def example() -> None:
    """Demonstrates a simple asynchronous behavior."""
```

---

## 🚀 How to Use

Clone the repository:

```bash
git clone <your-repo-link>
cd <repo-name>
```

Run files:

```bash
./filename.py
```

---

## 🧪 Code Style

Check your code:

```bash
pycodestyle .
```

---

## 📚 Resources

* asyncio documentation
* PEP 530 (Async Comprehensions)
* Python typing documentation

---

## ✨ Author

* Hamsa Alammar
