## Setup Python
- Setup VS Code [https://code.visualstudio.com/download]
- Install Python [https://www.python.org/downloads/]
- Create a file with '.py' extension (eg. `test.py`)
- Run the file using py as prefix (eg. `py test.py`)
- Alternatively, you can directly hit the run button in VS Code to execute Python code.


## VS Code Shortcuts
- Ctrl + / --> Comment multiple lines
- Use 'tab' to indent & 'Shift+Tab' to unindent
- Alt+Shift+DownArrow: To duplicate current line
- Modify multiple texts together: Click on Text, Use 'Alt', click on 2nd text, now you can edit them simultaneouly
- Settings --> Settings --> Commonly used --> Editor: Mouse Wheel Zoom (Enable it to zoom file using Ctrl + Mouse Wheel Up)
- Top --> Search --> ">Developer: Toggle Screencast Mode" --> (This will show the keyboard buttons used)

##	Python Basics
- Indentation helps Python to understand which lines are inside a block of code
-	Syntax ensures that code follows set of rules to be understood by computer
-	Python is a popular choice for data science & AI because it has large collection of libraries for data analysis & AI
	
##	Python Data Types
	Python is a dynamically typed language, so you don't need to define the data type
-	string             # name = "Panda"
-	integer            # age = 5 (integer with quotes are string)
-	float              # version = 1.2
-	boolean            # is_completed = True / False (First letter uppercase w/o quotes)
-	list               # [1,2,3,4,1,2] (changeable)
-	tuple              # (1,2,3,4) (fixed (cannot change))
-	set                # {1,2,3,4}
-	dictionary         # {"name": "panda", "age": 5}
<img width="405" height="460" alt="image" src="https://github.com/user-attachments/assets/9cb95642-d672-49f8-8cbc-f5312f34c11c" />

##	Variables
-	They are containers that store a value
-	Rules for defining a variable
-	a. Variables include letters, underscores & numbers
-	b. Variables can start with letter or underscore, but not a number
-	c. Variables are case-sensitive
-	d. Do not use the standard variables used in python (eg. if, else, for, while, etc)
	
##	Typecasting in Python
-	Typecasting is used to convert one data type to another
-	Eg: a. Let's say you want to convert string to integer number 5 (type: string) --> 5 (type: int)
```py
	a = "5"
	print(type(a)) --> O/P class 'string'
	b = int(a)
	print(type(b)) --> O/P class 'int'
```
	
-  Eg: b. We can also do vice-versa (integer to string)
```py
	a = 5
	b = str(a)
```

## Why Typecasting is required?
<img width="445" height="313" alt="image" src="https://github.com/user-attachments/assets/4cbb3b3d-3055-4034-bdeb-7499ae50a9e0" />
<img width="450" height="112" alt="image" src="https://github.com/user-attachments/assets/0df11fb8-c2ca-4a82-bf6a-c26012523aff" />


## User Input
<img width="446" height="191" alt="image" src="https://github.com/user-attachments/assets/f6482c73-c0b5-4e30-b92b-62f0871214f8" />

## Using new lines & tabs
<img width="446" height="191" alt="image" src="https://github.com/user-attachments/assets/e264961c-f507-4326-a69b-e1bd188c8bcc" />
	
	
## Comments
-	By default 'space' is a separator in Python
-	You can change the separator by defining it in "sep"
-	You can use end, to print what you require at the end of the line
- Keep it blank, to avoid bringing output to next lines (end="")
<img width="600" height="164" alt="image" src="https://github.com/user-attachments/assets/8b1d5cdc-8522-44ad-894e-7652a6c2c76e" />
	
## REPL in Python
-	Read Evaluate Process & Loop
-	This is where you can run default operation commands in Python
-	Simply type 'python' in the terminal & perform operations like +,-,/,*, etc
	
## Operators in Python
https://github.com/pandacloud1/python/blob/main/basics/01_basics.md#arithmetic-operators
- Arithmetric Operators: +, -, *, /, //, %
- Assignment Operators: a=30, a+=5 --> O/P: 35; a-=5 --> O/P: 25
- Conditional Operators: ==, !=, >, >=, <, <=
- Logical Operators: True/ False
![Uploading image.png…]()
 
### Note: 
a. Only True & True are "True", rest all combinations will give you a "False")
b. Only False or False are "False", rest all combinations will give you a "True")
c. We can reverse the output by using (not(True) --> False or vice versa

## Conditional Statements
  https://github.com/pandacloud1/python/blob/main/basics/statements.md
	
## Loops
  https://github.com/pandacloud1/python/blob/main/basics/loops.md
-	For loop
-	While loop --> ICAI
		
## STRING
  https://github.com/pandacloud1/python/blob/main/basics/06_strings.md
-	String index starts from 0
-	The last letter in string can be denoted with "-1"
-	The index can be found by adding length of string with the reverse index  [5+(-4) = 1]
```sh
	( P    A   N   D   A)
	( 0    1   2   3   4)
	(-5  -4  -3  -2  -1)
```

## String methods
- You can perform multiple functions on strings like upper, lower, capitalize, title, length
	
## FUNCTIONS
   What are functions?
-	Functions can help you create your own code
-	You define the function, where you create your own program
-	And then you need to call the function
-	Functions help you avoid repetition & can save lot of time with repeated lines of code
  https://github.com/pandacloud1/python/blob/main/advanced/01_functions.md
	
## Modules
   https://github.com/pandacloud1/python/blob/main/advanced/02_modules.md
	
## LISTS
   What are lists?
-	Lists are ordered & changeable list of data types
-	The list can contain string, integer, float or boolean
-	You can insert, remove or update any element in the list
-	Hence they are called mutable (changeable)

