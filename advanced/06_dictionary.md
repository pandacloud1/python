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

### Dictionary 
```py
student = {"name": "alexa", "age": 21, "location": "usa"}
### Printing key & values
print(student.keys())
print(student.values())
```
<img width="254" height="35" alt="image" src="https://github.com/user-attachments/assets/d62fba55-3cf5-4326-8cd4-3d4f1dae0087" />

### Removing key: value
```py
student = {"name": "alexa", "age": 21, "location": "usa"}

student.pop("age")
print(student)
```
<img width="242" height="23" alt="image" src="https://github.com/user-attachments/assets/1259ec22-aa99-44b0-9915-1214e6879eec" />
