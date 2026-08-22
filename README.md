# 🚀 Python Utility Toolkit

<div align="center">

## 🐍 A Menu-Driven Python Project

### Datetime • Mathematics • Random Data • UUID • File Handling • Custom Modules

**Made with Python 🐍**

</div>

---

## 📖 About The Project

**Python Utility Toolkit** is a menu-driven Python application that combines multiple useful Python concepts into one interactive project.

The application allows users to perform different operations from a simple menu system. It demonstrates the use of Python built-in libraries, custom modules, file handling, loops, conditional statements, and functions.

This project is designed to provide practical experience with modular programming and different Python utilities.

---

# ✨ Features

## 📅 1. Datetime and Time Operations

This section provides different date and time-related operations.

Available features:

* 🕒 Display Current Date and Time
* 📆 Format Date and Time
* ⏱️ Stopwatch
* ⏳ Countdown Timer

The project uses:

```python
from datetime import datetime
import time
```

---

## 🧮 2. Mathematical Operations

The project uses a custom module called `math_module.py`.

Available mathematical operations:

* 🔢 Calculate Factorial
* 💰 Calculate Compound Interest
* 📐 Trigonometric Calculations

  * Sine
  * Cosine
  * Tangent
* ⭕ Calculate Area of Circle

The Python `math` module is used to perform these calculations.

---

## 🎲 3. Random Data Generation

The application can generate random data using Python's `random` module.

Features include:

* Random Number Generation
* Random Choice from a List

Example programming language choices:

```text
Python
Java
C++
```

---

## 🆔 4. UUID Generation

The project can generate a unique identifier using:

```python
uuid.uuid4()
```

Each generated UUID is intended to be unique.

---

## 📁 5. File Operations

The project includes a custom module named `file_module.py`.

Available file operations:

* ✍️ Write Data to a File
* 📖 Read Data from a File
* ➕ Append New Data

The data is stored in:

```text
data.txt
```

---

## 🔍 6. Module Attribute Explorer

The project demonstrates the use of Python's `dir()` function.

The program displays available attributes and functions from the `random` module.

```python
print(dir(random))
```

---

## 🚪 7. Exit Option

The user can safely exit the application using the Exit option.

The program displays a thank-you message before terminating.

---

# 📂 Project Structure

```text
project_7/
│
├── 📄 __init__.py
├── 📄 main.py
├── 📄 helper.py
├── 📄 math_module.py
├── 📄 file_module.py
├── 📄 data.txt
│
├── 📦 Compiled Python Files
│   ├── __init__.cpython-311.pyc
│   ├── custom_modules.cpython-311.pyc
│   ├── datetime_utils.cpython-311.pyc
│   ├── dynamic_explorer.cpython-311.pyc
│   ├── file_module.cpython-311.pyc
│   ├── helper.cpython-311.pyc
│   ├── math_module.cpython-311.pyc
│   ├── math_utils.cpython-311.pyc
│   ├── random_utils.cpython-311.pyc
│   └── uuid_utils.cpython-311.pyc
│
└── 📄 README.md
```

---

# 🖥️ Main Menu

When the program starts, the following menu is displayed:

```text
Choose an option:

1. Datetime and Time Operations
2. Mathematical Operations
3. Random Data Generation
4. Generate Unique Identifier (UUID)
5. File Operations (Custom Module)
6. Explore Module Attributes (dir())
7. Exit
```

The user enters a number to select the required operation.

---

# 🛠️ Technologies Used

| Technology        | Purpose                             |
| ----------------- | ----------------------------------- |
| 🐍 Python         | Main Programming Language           |
| 📅 datetime       | Date and Time Operations            |
| ⏱️ time           | Stopwatch and Countdown             |
| 🧮 math           | Mathematical Calculations           |
| 🎲 random         | Random Data Generation              |
| 🆔 uuid           | Unique Identifier Generation        |
| 📁 File Handling  | Read, Write and Append Data         |
| 📦 Custom Modules | Modular Programming                 |
| 📂 GitHub         | Project Hosting and Version Control |

---

# ▶️ How to Run the Project

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/kukadiyakrisha08-web/project_7.git
```

## 2️⃣ Open the Project Folder

```bash
cd project_7
```

## 3️⃣ Run the Program

```bash
python main.py
```

Make sure Python is installed on your system before running the project.

---

# 💻 Sample Output

Below is an example of how the application works.

```text
========================================
      WELCOME TO PYTHON UTILITY TOOLKIT
========================================

Choose an option:

1. Datetime and Time Operations
2. Mathematical Operations
3. Random Data Generation
4. Generate Unique Identifier (UUID)
5. File Operations (Custom Module)
6. Explore Module Attributes (dir())
7. Exit

Enter your choice: 2
```

---

## 🧮 Mathematical Operation Example

```text
Mathematical Operations

1. Calculate Factorial
2. Compound Interest
3. Trigonometric Calculations
4. Area of Circle
5. Back

Enter choice: 1

Enter Number: 5

Factorial = 120
```

---

## 📅 Datetime Example

```text
Datetime and Time Operations

1. Display Current Date and Time
2. Format Date
3. Stopwatch
4. Countdown Timer
5. Back

Enter choice: 1

Current Date and Time:
2026-08-22 10:30:45
```

> The displayed date and time will be different depending on when the program is executed.

---

## 🎲 Random Data Example

```text
Random Data Generation

Random Number: 57

Random Choice: Python
```

> Random values may be different every time the program runs.

---

## 🆔 UUID Example

```text
Generated UUID:

550e8400-e29b-41d4-a716-446655440000
```

> A new UUID value can be generated each time the option is selected.

---

## 📁 File Operation Example

```text
File Operations

1. Write File
2. Read File
3. Append File
4. Back

Enter choice: 1

Enter text: Hello, Python!

Data Written Successfully
```

---

# 📚 Code Explanation

## 🔹 `main.py`

The `main.py` file is the main controller of the application.

It imports the required built-in libraries:

```python
from datetime import datetime
import time
import random
import uuid
```

It also imports custom modules:

```python
from modules import file_module
from modules import math_module
from modules.helper import welcome
```

The main program runs continuously using:

```python
while True:
```

The program displays the menu and waits for user input.

Based on the selected option, the program uses `if`, `elif`, and `else` statements to perform the appropriate operation.

For example:

```python
elif choice == "2":
    math_module.menu()
```

This calls the mathematical operations menu from the custom `math_module.py` file.

---

## 🔹 Datetime Operations

The current date and time are displayed using:

```python
datetime.now()
```

The date can be formatted using:

```python
datetime.now().strftime("%d-%m-%Y %H:%M:%S")
```

---

## 🔹 Stopwatch

The stopwatch records the start and end time.

```python
start = time.time()

# User stops the stopwatch

end = time.time()
```

The elapsed time is calculated by:

```python
end - start
```

---

## 🔹 Countdown Timer

The countdown timer accepts the number of seconds from the user.

It decreases the value every second using:

```python
time.sleep(1)
```

The timer continues until the value reaches zero.

---

## 🔹 `math_module.py`

The `math_module.py` file contains a separate menu for mathematical calculations.

It imports:

```python
import math
```

### Factorial

```python
math.factorial(n)
```

### Compound Interest

The amount is calculated using:

```python
amount = p * (1 + r / 100) ** t
```

The compound interest is:

```python
amount - p
```

### Trigonometric Calculations

The angle is converted into radians before calculation:

```python
math.sin(math.radians(angle))
math.cos(math.radians(angle))
math.tan(math.radians(angle))
```

### Area of Circle

```python
math.pi * r * r
```

---

## 🔹 `file_module.py`

The `file_module.py` file handles different file operations.

### Write File

The user enters text, and the program writes it to `data.txt`.

```python
f = open("data.txt", "w")
f.write(text)
f.close()
```

### Read File

The program reads and displays the contents of the file.

```python
f = open("data.txt", "r")
print(f.read())
f.close()
```

### Append File

New text can be added without removing the existing content.

```python
f = open("data.txt", "a")
f.write("\n" + text)
f.close()
```

The module also handles a missing file using `try-except`.

---

## 🔹 Random Module

The program generates a random number using:

```python
random.randint(1, 100)
```

It can also select a random programming language:

```python
random.choice(["Python", "Java", "C++"])
```

---

## 🔹 UUID Module

A unique identifier is generated using:

```python
uuid.uuid4()
```

---

## 🔹 `dir()` Function

The program uses:

```python
dir(random)
```

This displays the available attributes and functions of the `random` module.

---

# 📊 Results & Insights

## ✅ Modular Programming

The project successfully separates different functionalities into individual Python files.

Examples include:

* `main.py`
* `math_module.py`
* `file_module.py`
* `helper.py`

This makes the project more organized, reusable, and easier to understand.

---

## ✅ Interactive Menu System

The menu-driven interface allows the user to select different operations easily.

The use of nested menus also helps organize related features such as:

* Datetime Operations
* Mathematical Operations
* File Operations

---

## ✅ Practical Use of Python Libraries

This project demonstrates practical usage of multiple built-in Python libraries.

| Module     | Usage                               |
| ---------- | ----------------------------------- |
| `datetime` | Display and format date and time    |
| `time`     | Stopwatch and countdown timer       |
| `math`     | Mathematical calculations           |
| `random`   | Random number and choice generation |
| `uuid`     | Generate unique identifiers         |

---

## ✅ File Handling Results

The file module successfully performs:

* Writing user data
* Reading saved data
* Appending new data

This demonstrates how Python can be used for basic data storage using text files.

---

## 💡 Key Learnings

Through this project, the following Python concepts were explored:

* ✔ Functions
* ✔ Python Modules
* ✔ Custom Modules
* ✔ Built-in Modules
* ✔ User Input
* ✔ Conditional Statements
* ✔ `while` Loops
* ✔ Nested Menus
* ✔ File Handling
* ✔ Exception Handling
* ✔ Date and Time Operations
* ✔ Mathematical Calculations
* ✔ Random Data Generation
* ✔ UUID Generation
* ✔ Module Exploration using `dir()`

---

# 🎯 Conclusion

The **Python Utility Toolkit** successfully combines multiple important Python concepts into a single interactive application.

The project demonstrates how built-in Python libraries and custom modules can work together to create an organized and reusable program.

It provides practical experience with:

* Modular Programming
* File Handling
* Mathematical Calculations
* Date and Time Operations
* Random Data Generation
* UUID Generation
* Interactive Menu Systems

This project serves as a useful example of applying multiple Python concepts in one structured application.

---

# ⚠️ Note About `.pyc` Files

The repository may contain `.pyc` files generated automatically by Python.

These files are compiled versions of Python code and are generally not required to run the project from source files.

For future projects, these files can be ignored using a `.gitignore` file:

```gitignore
__pycache__/
*.pyc
```

---

# 👩‍💻 Author

## **Krisha Kukadiya**

🐍 Python Developer & Student

GitHub: **@kukadiyakrisha08-web**

---

<div align="center">

# ⭐ Thank You for Visiting!

### If you like this project, don't forget to give it a Star ⭐

**Made with ❤️ using Python 🐍**

</div>
