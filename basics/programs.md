## Sample Programs

### Check eligibility to vote
```py
age = int(input("Enter your age: "))
if age >= 18:
    print("You are elgible to vote")
else:
    print("You are not eligible to vote")
```

### Check BMI
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
