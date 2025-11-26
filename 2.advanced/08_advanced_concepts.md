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
  - It follows the DRY (Don't repeat yourself) principle
  - Without decorator: Imagine you want logging in 50 functions, and if tomorrow the logging logic changes? You must update all 50 functions again.
  - Provides clean and readable code
  - Replace/modify the main function behaviour if required
  - Decorators can help you to check token before running function (Authentication)
  - It help you to verify permissions (Authorization)
  - Retry failed calls, store results, open/close sessions, etc

Decorator & Wraper
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


"""
Imagine your my_line() function is a gift [my_line() --> func].
- A decorator is the gift wrapping process.
- my_line() or func = the original gift
- wrapper = wrapped gift with decoration

The return wrapper returns the wrapped gift.
"""
```
<img width="412" height="125" alt="image" src="https://github.com/user-attachments/assets/ad9747a7-8ec3-45b8-bf6c-4310c88fd7d9" />

Decorator & Wrapper (Calling function multiple times)
```py
def decorator(func):
    def wrapper():
        print("We are starting the main function...!")
        func()   # run your function once
        print("Running it again as a modification!")  # <-- NEW
        func()   # run it again
        print("Function executed successfully!")
    return wrapper

def my_line():
    print("-------------------------")
    print("THIS IS MY MAIN FUNCTION")
    print("-------------------------")

f = decorator(my_line)
f()
```
<img width="413" height="231" alt="image" src="https://github.com/user-attachments/assets/8c61e495-4ad1-4977-a75f-07a5ed9f41fa" />

