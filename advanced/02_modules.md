## MODULES
- Modules are used to import somebody else's code
- They are of two types: Build-in modules & external modules
- Build-in modules can be found here [https://docs.python.org/3/py-modindex.html]
- You can write you own modules & import them
- External modules can be installed via 'pip' (eg. pip install requests, requests module is used to fetch online urls)
- The dependency py files will be saved locally in your system
- Commonly used modules: requests, pandas, numpy, math, os, sys, boto3, botocore, etc.

### Math module (to get square root)
```py
import math
print(math.sqrt(16))
```
<img width="39" height="19" alt="image" src="https://github.com/user-attachments/assets/6d4225f4-e2ec-45a0-8eea-3d85bb4d053e" />

### Simple 'Hello World' module
module.py
```py
### Define module
### File name: mymodule.py
def hello():
    print("Hello World")
```
main.py
```py
import mymodule
mymodule.hello()
```
<img width="92" height="19" alt="image" src="https://github.com/user-attachments/assets/d184966d-5ec3-4d2b-a966-15e5e51e06ec" />

### Sum module (using sum function)
Sum function
```py
# File name: module.py
def sum(a,b,c):
    x = a+b+c
    print (x)
```
Main module
```py
import module
module.sum(1,2,3)
```
<img width="29" height="21" alt="image" src="https://github.com/user-attachments/assets/ad715f53-300c-4367-9810-c118af76f6c7" />

### Requests module (used for external modules)
```py
# First install requests using 'pip install requests'
import requests
r = requests.get("https://www.example.com")
print(r.text)
```
<img width="575" height="100" alt="image" src="https://github.com/user-attachments/assets/e34d5877-c260-4988-a29d-858ec6694077" />
