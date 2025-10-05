# 🧮 Assignment 5 - Advanced Modular Calculator

![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Tests](https://img.shields.io/badge/tests-passing-success)

**Author:** Muhammad Arham  
**Date:** October 2025  

---

## 📖 Project Overview

This project is a **professional-grade, modular calculator application** built with **Python**.  
It integrates **advanced design patterns**, **persistent data management using pandas**, and **automated CI/CD testing with GitHub Actions**.

The goal of this project is to demonstrate the use of clean architecture, modular design, and full test automation while applying real-world software development principles.

---

## 🚀 Key Features

- 🧩 **Design Patterns**
  - **Factory Pattern** – Creates operation objects dynamically.
  - **Strategy Pattern** – Defines interchangeable algorithms for operations.
  - **Observer Pattern** – Reacts to calculation events (logging, auto-saving).
  - **Memento Pattern** – Enables undo and redo functionality.
  - **Facade Pattern** – Simplifies interactions between multiple components.

- ⚙️ **Advanced Operations**
  - Addition  
  - Subtraction  
  - Multiplication  
  - Division  
  - Power  
  - Root  

- 🧠 **Error Handling**
  - Implements **LBYL (Look Before You Leap)** and **EAFP (Easier to Ask Forgiveness than Permission)** paradigms.
  - Graceful handling of invalid inputs and division by zero.

- 📊 **Persistent Data Management**
  - Uses **pandas DataFrame** for maintaining and saving calculation history.
  - Supports auto-saving and loading history from CSV files.

- ⚡ **Configuration System**
  - Uses `.env` and **environment variables** for flexible configuration.
  - Validates missing or invalid configurations automatically.

---

## 📂 Project Structure

assignment5/
│── app/
│ ├── calculator_repl.py # REPL interface (main program loop)
│ ├── calculation.py # Core calculation and operation logic
│ ├── calculator_config.py # Configuration management
│ ├── calculator_memento.py # Memento pattern (undo/redo state)
│ ├── exceptions.py # Custom exception handling
│ ├── history.py # History management with pandas
│ ├── input_validators.py # Input validation logic
│ └── operations.py # Arithmetic operation definitions
│
│── tests/ # Unit and parameterized tests
│── requirements.txt # Python dependencies
│── .github/workflows/python-app.yml # GitHub Actions CI workflow
│── README.md # Documentation (this file)

yaml
Copy code

---

## ▶️ Run Instructions

### 1️⃣ Clone the repository
```bash
git clone git@github.com:arhamidrees63/assignment5.git
cd assignment5
2️⃣ Create and activate a virtual environment
bash
Copy code
python3 -m venv venv
source venv/bin/activate   # For Mac/Linux
venv\Scripts\activate      # For Windows
3️⃣ Install dependencies
bash
Copy code
pip install -r requirements.txt
4️⃣ Run the calculator
bash
Copy code
python app/calculator_repl.py
🧪 Testing and Coverage
Run all tests with coverage:

bash
Copy code
pytest --cov=app --cov-report=term-missing
The GitHub Actions CI pipeline automatically runs these tests on every push and enforces 100% test coverage.

Coverage results are displayed as badges (see top of README).

💾 Persistent History
All calculations are stored using pandas.DataFrame and saved in .csv format.
When you restart the calculator, previous history automatically loads.

Example saved data:

sql
Copy code
operation,operand_a,operand_b,result,timestamp
add,10,5,15,2025-10-05 12:45:00
power,2,3,8,2025-10-05 12:47:15
🧰 Available Commands
Command	Description
help	Display usage instructions
history	Show all previous calculations
undo	Undo the last operation
redo	Redo an undone operation
save	Save calculation history to CSV
load	Load saved history
clear	Clear all history
exit	Exit the calculator

🧠 Learning Outcomes
Apply advanced OOP principles and design patterns.

Implement data persistence using pandas.

Practice test-driven development (TDD) with full coverage.

Build and automate CI/CD pipelines using GitHub Actions.

Develop a clean, modular, and maintainable Python codebase.

🏁 Acknowledgments
This project was completed as part of IS601 – Advanced Systems Development coursework.
It demonstrates the combination of theoretical design patterns and practical coding applications.