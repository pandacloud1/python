## FUNCTIONS
- Functions help you to write your own code
- You need to define the function & call it to execute
- They are used for reusability & modularity
- 'Return' can help you store values in a variable

### Sum function
```py
def sum(a,b,c):
    x = a+b+c
    print (x)
sum(1,2,3)
```
<img width="32" height="20" alt="image" src="https://github.com/user-attachments/assets/bce8b174-518c-428e-8c6b-8bb699f381bb" />

### Multiply function
Using positional arguments
```py
def multiply(a,b,c):
    x = a*b*c
    print (x)
multiply(4,5,6)
```

Using default arguments
```py
def multiply(a=4,b=5,c=6):
    x = a*b*c
    print (x)
multiply()
```
<img width="37" height="21" alt="image" src="https://github.com/user-attachments/assets/0cc46e95-5b39-40e3-b997-31547abb9a02" />

Overwriting default arguments
```py
def multiply(a=4,b=5,c=6):    # default arguments
    x = a*b*c
    print (x)
multiply(10,11,12)            # overwriting arguments
```
<img width="43" height="20" alt="image" src="https://github.com/user-attachments/assets/401b4ac1-762a-44a2-bd68-8bb93279b4dc" />


### Average of 3 numbers
```py
def average(a,b,c):     # here a,b,c are parameters
    avg = (a+b+c)/3
    print(avg)

average(1,2,3)          # here 1,2,3 are arguments
average(4,5,6)
average(7,8,9)
```
<img width="71" height="49" alt="image" src="https://github.com/user-attachments/assets/44fe6b6f-2c82-41b7-86a7-d5aeef04d25d" />

### Using return to store value in variable
```py
def average(a,b,c):
    avg = (a+b+c)/3
    return avg

a1 = average(1,2,3)
a2 = average(4,5,6)
a3 = average(7,8,9)
print(a1,a2,a3)
```
<img width="84" height="19" alt="image" src="https://github.com/user-attachments/assets/c21a41b2-441c-4a3a-b0a9-0f9f183f8eca" />
