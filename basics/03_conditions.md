## Conditional Statements

### If-else (Check eligibility to vote)
```py
age = int(input("Enter your age: "))
if age >= 18:
    print("You are elgible to vote")
else:
    print("You are not eligible to vote")
```

### Check if number is even or odd
```py
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Number is Even")
else:
    print("Number is Odd")
```

### Check if number is positive, negative, or zero
```py
num = int(input("Enter a number: "))
if num > 0:
    print("Number is positive")
elif num == 0:
    print("Number is zero")
else:
    print("Number is negative")
```

### If-elif-else statement (Check BMI)
```py
weight = float(input("Enter weight in kg: "))
height = float(input("Enter height in metres: "))

bmi = (weight/height**2)
print (f"bmi is {bmi}")

if (bmi>30):
    print("You are obese")
elif (25<bmi<=30):
    print("You are overweight")
elif (18<=bmi<25):
    print("You have an ideal weight")
else:
    print("You are underweight")
```

### Case statement (Lucky number)
```py
a = int(input("Enter any number from 1 to 5: "))

match a:
    case 1: 
        print("You won a toy gun!")
    case 2:
        print("You won Nike shoes!")
    case 3:
        print("You won free movie ticket!")
    case 4:
        print("You won a vacation package!")
    case _:
        print("Sorry! Better luck next time")
```
