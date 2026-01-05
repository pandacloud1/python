## Setup Python

* Set up VS Code: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)
* Install Python: [https://www.python.org/downloads/](https://www.python.org/downloads/)
* Create a file with a `.py` extension (e.g., `test.py`)
* Run the file using `py` as a prefix (e.g., `py test.py`)
* Alternatively, you can directly click the **Run** button in VS Code to execute Python code

## VS Code Shortcuts

* `Ctrl + /` → Comment/uncomment multiple lines
* Use `Tab` to indent & `Shift + Tab` to unindent
* `Alt + Shift + Down Arrow` → Duplicate the current line
* Modify multiple texts together:

  * Click on text
  * Hold `Alt` and click on another text
  * Edit both simultaneously
* Settings → Settings → Commonly Used → **Editor: Mouse Wheel Zoom**

  * Enable it to zoom files using `Ctrl + Mouse Wheel`
* Top → Search → `>Developer: Toggle Screencast Mode`

  * Shows keyboard shortcuts on screen

## Python Basics

* Indentation helps Python understand which lines belong to a block of code
* Syntax ensures the code follows a set of rules understood by the computer
* Python is widely used in **Data Science & AI** due to its large collection of libraries

## Python Data Types

Python is a **dynamically typed language**, so you don’t need to declare data types explicitly.

* `string`       → `name = "Panda"`
* `integer`      → `age = 5` (numbers inside quotes become strings)
* `float`        → `version = 1.2`
* `boolean`      → `is_completed = True / False` (First letter uppercase, no quotes)
* `list`         → `[1, 2, 3, 4]` (changeable)
* `tuple`        → `(1, 2, 3, 4)` (fixed / immutable)
* `set`          → `{1, 2, 3, 4}`
* `dictionary`   → `{"name": "panda", "age": 5}`

<img width="405" height="460" alt="image" src="https://github.com/user-attachments/assets/9cb95642-d672-49f8-8cbc-f5312f34c11c" />

## Variables

* Variables are containers used to store values

**Rules for defining variables:**

* Variables can include letters, underscores, and numbers
* They must start with a letter or underscore (not a number)
* Variables are case-sensitive
* Do not use Python keywords (e.g., `if`, `else`, `for`, `while`)

## Typecasting in Python

* Typecasting is used to convert one data type into another

### Example: String to Integer

```py
a = "5"
print(type(a))   # Output: <class 'str'>
b = int(a)
print(type(b))   # Output: <class 'int'>
```

### Example: Integer to String

```py
a = 5
b = str(a)
```

## Why Typecasting is Required?
- The below program which is a bit lengthy
<img width="445" height="313" alt="image" src="https://github.com/user-attachments/assets/4cbb3b3d-3055-4034-bdeb-7499ae50a9e0" />

- It will get simplified by using typecasting
<img width="450" height="112" alt="image" src="https://github.com/user-attachments/assets/0df11fb8-c2ca-4a82-bf6a-c26012523aff" />

## User Input

* The `input()` function is used to take input from the user
* By default, input is treated as a **string**

<img width="446" height="191" alt="image" src="https://github.com/user-attachments/assets/f6482c73-c0b5-4e30-b92b-62f0871214f8" />

## Using New Lines & Tabs

* `\n` → New line
* `\t` → Tab space
<img width="450" height="152" alt="image" src="https://github.com/user-attachments/assets/63b00c11-8de9-44bc-927f-3af98b00f9f5" />

## Comments & Print Formatting

* By default, **space** is used as a separator in `print()`
* You can change the separator using `sep`
* Use `end` to control what prints at the end of the line
* Use `end=""` to avoid moving output to the next line

<img width="600" height="164" alt="image" src="https://github.com/user-attachments/assets/8b1d5cdc-8522-44ad-894e-7652a6c2c76e" />

## REPL in Python

* REPL stands for **Read, Evaluate, Process, Loop**
* Used to quickly test Python commands
* Type `python` in the terminal and perform operations like `+`, `-`, `*`, `/`

## Operators in Python

Reference:
[https://github.com/pandacloud1/python/blob/main/basics/01_basics.md#arithmetic-operators](https://github.com/pandacloud1/python/blob/main/basics/01_basics.md#arithmetic-operators)

* **Arithmetic Operators**: `+`, `-`, `*`, `/`, `//`, `%`
* **Assignment Operators**:

  * `a = 30`
  * `a += 5` → Output: 35
  * `a -= 5` → Output: 25
* **Conditional Operators**: `==`, `!=`, `>`, `>=`, `<`, `<=`
* **Logical Operators**: `and`, `or`, `not`

### Note:

* Only `True and True` results in `True`
* Only `False or False` results in `False`
* `not` reverses the output

## Conditional Statements

Reference:
[https://github.com/pandacloud1/python/blob/main/basics/statements.md](https://github.com/pandacloud1/python/blob/main/basics/statements.md)

**What are conditional statements?**

* They are used to make decisions in code
* Based on conditions like `if`, `elif`, and `else`
* The program executes different blocks of code based on conditions

## Loops

Reference:
[https://github.com/pandacloud1/python/blob/main/basics/loops.md](https://github.com/pandacloud1/python/blob/main/basics/loops.md)

**What are loops?**

* Loops are used to repeat a block of code multiple times

Types:

* `for` loop
* `while` loop

## STRING

Reference:
[https://github.com/pandacloud1/python/blob/main/basics/06_strings.md](https://github.com/pandacloud1/python/blob/main/basics/06_strings.md)

* String index starts from `0`
* The last character can be accessed using `-1`
* Index can be calculated using string length

```text
( P    A    N    D    A )
( 0    1    2    3    4 )
(-5   -4   -3   -2   -1)
```

## String Methods

* Used to perform operations on strings
* Examples: `upper()`, `lower()`, `capitalize()`, `title()`, `len()`

## FUNCTIONS

Reference:
[https://github.com/pandacloud1/python/blob/main/advanced/01_functions.md](https://github.com/pandacloud1/python/blob/main/advanced/01_functions.md)

**What are functions?**

* Functions allow you to group reusable code
* You define a function once and call it whenever needed
* Helps avoid repetition and makes code cleaner

## Modules

Reference:
[https://github.com/pandacloud1/python/blob/main/advanced/02_modules.md](https://github.com/pandacloud1/python/blob/main/advanced/02_modules.md)

**What are modules?**

* Modules are Python files that contain reusable code
* They help organize code into separate files
* Examples: `math`, `os`, `sys`

## LISTS

**What are lists?**

* Lists are ordered and changeable collections of data
* They can store different data types
* You can add, remove, or update elements
* Lists are **mutable** (changeable)
* Add **small code examples** under each topic
* Convert it into a **training-friendly format** (Day 1 / Day 2 style)
