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

### Working on parent class & inheritance
```py
class Animal:
    def __init__ (self, name):
        self.name = name
    def speak(self):
        print("Speaking now...")

class Dog(Animal):
    def speak(self):
        print("Bow bow")

a = Animal("Dog")
a.speak()

d = Dog("Bruno")
d.speak()
```
<img width="109" height="32" alt="image" src="https://github.com/user-attachments/assets/6f08a925-d951-4728-835b-9fb45eb35df4" />

### Method Overriding & Operator Overloading
```py
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def sum(self, p):
        return Point((self.x+p.x), (self.y+p.y))
    def print_point(self):
        return (f"X is {self.x} & Y is {self.y}")

p1 = Point(3,2)
p2 = Point(6,9)

p = p1.sum(p2)
print(p.print_point())
```

OR

```
class Point:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def sum(self, p):
        return Point((self.x+p.x), (self.y+p.y))
    def print_point(self):
        return (f"X is {self.x} & Y is {self.y}")
    def __add__ (self, p):
        return Point((self.x+p.x),(self.y+p.y))

p1 = Point(3,2)
p2 = Point(6,9)

p = p1+p2              # You cannot directly add it, instead need to use "__add__" function
print(p.print_point())
```
<img width="117" height="19" alt="image" src="https://github.com/user-attachments/assets/1482aa6b-0f3c-410e-997a-270fda043c74" />
