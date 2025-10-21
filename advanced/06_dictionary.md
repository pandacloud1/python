## DICTIONARY
- Dictionary stores key-value pair for faster lookup
- You can change the values in the dictionary (mutuable)

### Dictionary example
```py
student = {"name": "alexa", "age": 21, "location": "usa"}
print(student)
print(student["name"])
print(student["age"])
print(student["location"])
### Changing values (mutuable)
student["location"] = "australia"
print(student)
```
<img width="352" height="82" alt="image" src="https://github.com/user-attachments/assets/ea7e21f8-dfe3-49ce-8bdd-115c2b7eee55" />

### Printing keys & values
```py
student = {"name": "alexa", "age": 21, "location": "usa"}
### Printing key & values
print(student.keys())
print(student.values())
```
<img width="254" height="35" alt="image" src="https://github.com/user-attachments/assets/d62fba55-3cf5-4326-8cd4-3d4f1dae0087" />

### Removing data
```py
student = {"name": "alexa", "age": 21, "location": "usa"}

student.pop("age")
print(student)

student.clear()
print(student)
```
<img width="245" height="38" alt="image" src="https://github.com/user-attachments/assets/ae747a8f-3e3b-4b0b-b09b-8f132ab2e773" />

### Dictionary comprehension
### Table of 5
```py
tab = {i: 5*i for i in range(1,11)}
print(tab)
```
<img width="471" height="20" alt="image" src="https://github.com/user-attachments/assets/c498844e-1e2d-40c6-984c-8b8c852d944f" />

### Square of numbers (1-10)
```py
sq = {n: n**2 for n in range(1,11)}
print(sq)
```
<img width="456" height="20" alt="image" src="https://github.com/user-attachments/assets/31b2ef59-ab40-4f5d-99db-66bd1181393f" />

