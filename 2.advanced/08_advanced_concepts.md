## DECORATORS
- "Decorator" is a way to extend behaviour of functions
- There is no need to alter the code
- It can take another function as an argument
- We need to "wrap" the orginal function with additional logic
- This wrapping is done by defining an inner function (often called a "wrapper") within the decorator.
- So you have "decorator" at the top and "wrapper" inside it

```py
def decorator (func):
    def wrapper():
      print ("This is the first line")
      func ()
      print ("This is the third line")
    return wrapper

def my_line():
    print("This is the second line")

f = decorator(my_line)
f()
```
<img width="265" height="83" alt="image" src="https://github.com/user-attachments/assets/ad318e1a-003c-453b-942d-2b3b987792ee" />

