<div align="center">
  <h1>⚡ UV — The Blazing-Fast Python Project Manager</h1>
  <p>🚀 A blazing-fast, modern Python package and dependency manager that combines the best of Poetry, pip, and pyenv — all in one tool.</p>

[![GitHub Repo stars](https://img.shields.io/github/stars/marcellin-d/uv?style=flat-square&color=yellow)](https://github.com/marcellin-d/uv/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/marcellin-d/uv?style=flat-square)](https://github.com/marcellin-d/uv/network/members)
[![GitHub last commit](https://img.shields.io/github/last-commit/marcellin-d/uv?style=flat-square&color=brightgreen)](https://github.com/marcellin-d/uv/commits/main)
[![License](https://img.shields.io/github/license/marcellin-d/uv?style=flat-square)](https://github.com/marcellin-d/uv/blob/main/LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue?style=flat-square)](https://www.python.org/)

</div>
<br />

<img width="100%" alt="UV Cover Image" src="./cover_image.png">

---

## 🚀 Introduction

Meet **UV**, the new powerhouse in Python project management.  
Forget the days of juggling `poetry`, `requirements.txt`, and `pyenv` — **UV does it all**, and it does it _blazingly fast_.

With UV, you can:

- Initialize and manage Python projects effortlessly
- Add, lock, and sync dependencies instantly
- Manage multiple Python versions
- Run commands in isolated environments
- Enjoy unmatched speed and simplicity

---

## 🧩 Installation

You can install UV in several ways — via **curl**, **pip**, or **PowerShell** (for Windows).

Here’s an example using **curl**:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Once installed, verify with:

```bash
uv --version
```

---

## ⚙️ Project Initialization

To create a new project, simply run:

```bash
uv init
```

This will generate a `pyproject.toml` file that includes:

- Project metadata
- Dependencies
- Python version

You can then edit or sync your environment as needed.

---

## 📦 Adding Dependencies

Adding packages is effortless:

```bash
uv add typer
```

To add development dependencies, use the `--dev` flag:

```bash
uv add pytest --dev
```

---

## 🧪 Running Commands

Let’s set up a simple test:

```bash
mkdir tests
echo "def test_main(): assert True" > tests/test_main.py
```

Then run your tests inside UV’s virtual environment:

```bash
uv run pytest
```

✨ **Note:** UV automatically creates and manages a `.venv` for you.

---

## 🐍 Managing Python Versions

UV can install and switch between Python versions seamlessly.

Check your current version:

```bash
uv run python --version
```

To upgrade to Python 3.14:

1. Edit your `pyproject.toml`:

   ```toml
   requires-python = ">=3.14"
   ```

2. Sync the environment:
   ```bash
   uv sync
   ```

---

## ⚡ Performance

UV is _incredibly fast_.  
You can install large packages like **FastAPI**, **Jupyter**, and **Pandas** in seconds:

```bash
uv add fastapi jupyter pandas
```

Everything installs, resolves, and locks in under **2 seconds**. 🔥

---

## 🧰 Using `uvx` (Standalone Tools)

Need to run a one-off tool like **Ruff** for linting or formatting?  
No need to install it globally — just use `uvx`:

```bash
uvx ruff check
uvx ruff format
```

It runs tools in a **fully isolated environment** without touching your project dependencies.

---

## 🏁 Summary

With **UV**, you can:

- ✅ Initialize and manage projects
- ✅ Add & sync dependencies instantly
- ✅ Manage Python versions easily
- ✅ Run isolated environments
- ✅ Enjoy unmatched speed and simplicity

---

## 💬 Conclusion

**UV** redefines Python project management — it’s clean, fast, and powerful.  
Once you try it, it might just become your favorite Python tool.

> 🧡 Found this useful? Star ⭐ the repo and happy coding!

---

## ⚙️ Tech Stack (for this project)

- 🐍 Python 3.8+
- 📦 UV (Dependency & Environment Manager)
- 🧪 Pytest (for testing)
- 🪶 TOML Configuration
- 💾 SQLite (default lightweight database)
- 🧰 Git + GitHub for version control

---

## 📜 License

Licensed under the [MIT License](./LICENSE).
