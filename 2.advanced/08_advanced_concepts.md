## DECORATORS
- What is Decorator & Wrapper?
  - "Decorator" is a way to extend behaviour of functions
  - It is something that runs before and after the main function, without needing to modify the actual function
  - There is no need to alter the code
  - It can take another function as an argument
  - We need to "wrap" the orginal function with additional logic
  - This wrapping is done by defining an inner function (often called a "wrapper") within the decorator.
  - So you have "decorator" at the top and "wrapper" inside it

- Why Decorator?
  - There is no need to modify the main function
  - It follows the DRY principle
  - Provides clean and readable code
  - Replace/modify the main function behaviour if required
    
```py
def decorator(func):
    def wrapper():
        print("We are starting the main function...!")
        func()
        print("Function executed successfully!")    
    return wrapper

def my_line():
    print("-------------------------")
    print("THIS IS MY MAIN FUNCTION")
    print("-------------------------")

f = decorator(my_line)
f()
```
<img width="412" height="125" alt="image" src="https://github.com/user-attachments/assets/ad9747a7-8ec3-45b8-bf6c-4310c88fd7d9" />


