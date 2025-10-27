## CLASS, OBJECTS, ATTRIBUTES & METHODS
- Classes means a template
- Objects are created from the template
- Attributes represent features
- Methods represent actions
- Example:
  - Design of a house is a Class
  - Building the actual house is an Object
  - House features like rooms, doors and windows are Actions
  - Opening/closing doors, switch on/off lights are Methods

### Define class & object
```py
# define class
class Employee:
    company = "Panda Cloud"
   
    def salary(self):           # Here 'self' is mandatory
        return 150000

# define object                 # for class 'Employee'
e1 = Employee()
print(e1.company)               
print(e1.salary())              # here 'salary' method is called
```
<img width="83" height="34" alt="image" src="https://github.com/user-attachments/assets/d6a687b2-e25c-4cfd-8db0-954be6ca9a62" />

### Creating constructors
```py
class Employee:

    def __init__(self, name, age, salary):
        self.name = name
        self.age = age
        self.salary = salary
    
    def salary(self):
        print (self.salary())
    
    def info(self):
        print(f"Employee name is {self.name}, age is {self.age} & salary is {self.salary}")

e1 = Employee("alexa", 21, 123456)
print(e1.salary)
e1.info()
```
<img width="346" height="33" alt="image" src="https://github.com/user-attachments/assets/c0406bd9-a0a4-402a-a87d-c26224ea464f" />
