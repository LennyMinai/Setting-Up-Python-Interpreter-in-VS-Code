# 🐍 Setting Up Python Interpreter in VS Code

This repository documents the steps I followed to successfully run my first Python code in **Visual Studio Code (VS Code)** and fix the "Choose Interpreter" warning.

---

## 🚀 Goal

Help beginners (like myself) quickly fix the `"Select Interpreter"` issue in VS Code and start running Python code confidently.

---

## ✅ Prerequisites

- Visual Studio Code installed
- Python installed (from [python.org](https://www.python.org/))
- Basic knowledge of navigating your file system

---

## 🛍️ Steps I Followed

### 1. Opened VS Code and Tried to Run Python Code

After writing a simple Python script, I noticed a yellow exclamation mark on the bottom bar saying:

```
⚠️ Select Python Interpreter
```

---

### 2. Clicked “Select Interpreter”

- Clicked the **bottom-right warning** OR pressed `Ctrl + Shift + P`
- Selected: `Python: Select Interpreter`

---

### 3. No Interpreter Found? Got This Prompt

When the prompt showed:

- `Create virtual environment`
- `Enter interpreter path`

I realized VS Code wasn’t detecting Python automatically.

---

### 4. Checked if Python Was Installed

Opened the **integrated terminal** in VS Code and ran:

```bash
python --version
```
OR

```bash
py -3 --version
```

If this failed, I installed Python from [https://www.python.org/downloads](https://www.python.org/downloads) and ensured to tick ✅ **"Add Python to PATH"** during installation.

---

### 5. Manually Set Python Interpreter

If Python was installed but not visible:

- Pressed `Ctrl + Shift + P`
- Selected `Python: Select Interpreter` → `Enter interpreter path...` → `Find`
- Navigated to:
  ```
  C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python311\python.exe
  ```
- Clicked **Select**

---

### 6. (Optional) Created a Virtual Environment

Once the interpreter was selected:

- Pressed `Ctrl + Shift + P`
- Selected `Python: Create Environment`
- Chose `venv`
- Accepted default settings (environment created in `.venv` folder)

VS Code automatically activated the environment.

---

## 🔪 Final Check

- The exclamation mark disappeared ✅
- Bottom bar now showed selected interpreter (e.g., `Python 3.11.4 (.venv: venv)`)
- I could successfully run my script!

---

## 📁 Example Python Script

```python
print("Hello, Python World!")
```

---

## 📌 Notes

- Always make sure Python is added to your system `PATH`
- You can create separate virtual environments for each project using `.venv`
- Use `python -m venv .venv` from terminal if you prefer manual setup

---

## 🙌 Credits

Documented by: **LennyDevs**

Inspired by my first experience with Python on VS Code.
