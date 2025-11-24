## Python Basics

- Setup VS Code
- Install Python [https://www.python.org/downloads/]

### Printing message (file name: test.py)
```py
print ("Hello World")
```
<img width="301" height="62" alt="image" src="https://github.com/user-attachments/assets/d8961cc3-b70d-4946-bbb6-6bab21046584" /><br>
Alternatively, you can directly hit the run button in VS Code to execute python code.

### Multi-line comment
```py
'''
This is a multi-line comment
We need to use triple single quotes for same
You can keep on adding multiple lines
You can also Ctrl+/ in VS code
'''
```

### Using different separator (eg: /)
```py
# Using different separator (eg: /)
print("Hello Everyone","How are you?","Let's learn Python")
print("Hello Everyone","How are you?","Let's learn Python",sep="/")

# Using end
print("Hello Everyone", end="! ")
print("How are you", end="? ")
print("I am fine")
```
Output
```
Hello Everyone How are you? Let's learn Python
Hello Everyone/How are you?/Let's learn Python
Hello Everyone! How are you? I am fine
```

### Escape sequence characters
```
\n: new line
\t: tab
\\: backslash
\": Double quotes
\': Single quote
```
```py
print("Sr\tName\tAge\n1\t\"Alexa\"\t12\n2\t\"Ethan\"\t57")
```
Output
```sh
Sr   Name     Age
1    "Alexa"  12
2    "Ethan"  57
```

### Typecast (convert data types)
```py
# Example-1: Convert string to integer
a = "5"
print(type(a))
# --> O/P class 'string'
b = int(a)
print(type(b))
# --> O/P class 'int'

# Example-2: We can also do vice-versa (integer to string)
a = 5
b = str(a)
```

### Why Typecasting is Required?
```py
a = int(input("Enter first number: ")) # convert string --> integer
b = int(input("Enter second number: ")) # convert string --> integer
 
print("The sum is: ")
print(a+b)
```

### Arithmetic Operators
```py
a = 25
b = 2

print("Add", a + b)
print("Sub", a-b)
print("Mult", a*b)
print("Div/Quotient(decimal)", a/b)
print("FloorDiv/Quotient(int)", a//b)
print("Modulus/Remainder", a%b)
print("Exponential/Square", a**b)
```
Output
```
Add 27
Sub 23
Mult 50
Div/Quotient(decimal) 12.5
FloorDiv/Quotient(int) 12
Modulus/Remainder 1
Exponential/Square 625
```
<img width="216" height="121" alt="image" src="https://github.com/user-attachments/assets/5f6996a9-1120-4f4b-9b3a-a915b11c42a9" />
