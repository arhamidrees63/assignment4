# Assignment 4 - Command-Line Calculator

![Coverage](./coverage.svg)

## Author
**Muhammad Arham**  
Date: September 2025  

---

## 📖 Project Overview
This project is a modular, professional-grade **command-line calculator application** written in Python. It demonstrates clean architecture, modular design, error handling, unit testing, and continuous integration with GitHub Actions.

The calculator provides:
- A REPL (Read-Eval-Print Loop) interface.
- Arithmetic operations: addition, subtraction, multiplication, division, and power.
- Input validation and error handling (invalid inputs, division by zero, etc.).
- Calculation management through a `CalculationFactory`.
- Special commands:
  - `help` → Show usage instructions.
  - `history` → Display previously executed calculations.
  - `exit` → Quit the calculator.

---

## 📂 Project Structure
```text
assignment4/
│── app/
│   ├── calculator/       # REPL logic
│   ├── calculation/      # Calculation factory and base class
│   └── operation/        # Arithmetic operations
│── tests/                # Unit and parameterized tests
│── main.py               # Entry point for the calculator
│── requirements.txt      # Project dependencies
│── pytest.ini            # Pytest configuration
│── .coveragerc           # Coverage configuration
│── .github/workflows/    # GitHub Actions CI pipeline
▶️ Running the Application
Clone the repository:

bash
Copy code
git clone git@github.com:arhamidrees63/assignment4.git
cd assignment4
Create and activate a virtual environment:

bash
Copy code
python3 -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the calculator:

bash
Copy code
python main.py
🧪 Running Tests
Run all tests with coverage:

bash
Copy code
pytest --cov=app --cov-report=term-missing
⚙️ Continuous Integration
GitHub Actions automatically runs all tests on each push.

Enforces 100% test coverage.

Generates a coverage badge (see top of README).

✅ Learning Objectives
Apply OOP concepts (Encapsulation, Abstraction, Factory pattern).

Practice robust error handling (LBYL and EAFP).

Use modular design for clean, reusable code.

Implement unit + parameterized tests with pytest.

Automate testing and coverage enforcement via GitHub Actions.