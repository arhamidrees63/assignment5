# Assignment 5 – Advanced Modular Calculator

![Coverage](./coverage.svg)

## 👨‍💻 Author
**Muhammad Arham**  
Date: October 2025  

---

## 📖 Overview
This project is a **professional-grade command-line calculator** built with Python.  
It demonstrates the use of **advanced design patterns**, **persistent data handling**, and **automated testing with CI/CD**.

The calculator provides:
- Continuous **REPL interface**
- Arithmetic operations: `add`, `subtract`, `multiply`, `divide`, `power`, and `root`
- Full **undo/redo** history tracking using the **Memento Pattern**
- **Auto-saving history** to CSV files using **pandas**
- **Observer Pattern** for logging and event tracking
- **Strategy Pattern** for interchangeable operation execution
- **Factory Pattern** for object creation
- **Facade Pattern** to simplify subsystem access
- **dotenv configuration** for environment-based settings
- Rich commands:  
  `help`, `history`, `clear`, `undo`, `redo`, `save`, `load`, and `exit`

---

## 🗂️ Project Structure
assignment5/
│── app/
│ ├── calculator_repl.py # REPL interface for user interaction
│ ├── calculator.py # Core logic and Facade pattern
│ ├── calculation.py # Factory & Strategy patterns
│ ├── calculator_memento.py # Undo/Redo (Memento pattern)
│ ├── history.py # Observer for history tracking
│ ├── calculator_config.py # dotenv configuration management
│ ├── input_validators.py # Input validation and sanitization
│ ├── operations.py # Arithmetic operations
│ ├── exceptions.py # Custom error handling
│── tests/ # Unit and parameterized tests
│── .github/workflows/python-app.yml # CI pipeline
│── requirements.txt # Dependencies
│── README.md

yaml
Copy code

---

## ▶️ Running the Application
1. Clone the repository:
   ```bash
   git clone git@github.com:arhamidrees63/assignment5.git
   cd assignment5
Create and activate a virtual environment:

bash
Copy code
python3 -m venv venv
source venv/bin/activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the calculator:

bash
Copy code
python app/calculator_repl.py
🧪 Running Tests
Run all tests with coverage:

bash
Copy code
pytest --cov=app --cov-report=term-missing
⚙️ Continuous Integration
This project uses GitHub Actions for CI/CD.
Each push automatically:

Runs all tests

Enforces 100% coverage

Generates a coverage badge

🧠 Learning Objectives
Apply advanced OOP design patterns

Manage persistent data with pandas

Implement full test coverage and CI automation

Demonstrate maintainable, scalable modular code

🧩 Example Usage
ruby
Copy code
>> add 10 5
Result: 15.0

>> power 2 3
Result: 8.0

>> undo
Last action undone.

>> redo
Redo successful.

>> save
History saved to calculator_history.csv

>> exit
Exiting calculator. Goodbye!
🏁 End
This project combines design patterns, data management, and testing automation to simulate real-world software engineering standards.

yaml
Copy code

---

## ✅ Next Steps for You

1. Copy-paste that README into your repo.  
2. Run:
   ```bash
   git add README.md
   git commit -m "Update README for Assignment 5"
   git push origin main