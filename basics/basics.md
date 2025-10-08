## Python Basics

Printing message
```py
print ("Hello World")
```

Multi-line comment
```py
'''
This is a multi-line comment
We need to use triple single quotes for same
You can keep on adding multiple lines
# You can also Ctrl+/ in VS code
'''
```

Typecast (convert data types)
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

Why Typecasting is Required?
```py
a = int(input("Enter first number: ")) # convert string --> integer
b = int(input("Enter second number: ")) # convert string --> integer
 
print("The sum is: ")
print(a+b)
```

Check eligibility to vote
```py
age = int(input("Enter your age: "))
if age >= 18:
    print("You are elgible to vote")
else:
    print("You are not eligible to vote")
```
