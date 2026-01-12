## Simple calculator

``` py
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))

print ("Select operation to perform:\n'+' for addition\n'-' for subtraction\n'*' for multiplication\n'/' for division")

i = input("Enter operation: ")
match i:
  case '+': 
    print ("The sum is: ", a+b)
  case '-':
    print("The difference is: ", a-b)
  case '*':
    print("The product is : ", a*b)
  case '/':
    print("The division is : ", a/b)
  case _:
    print("Invalid input")
```
