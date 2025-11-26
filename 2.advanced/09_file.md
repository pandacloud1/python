## WORKING WITH FILES

### Reading a file in Python
```txt
### file.txt
### Simple text file
This is a test file.
We have created it, so that we can read it through python.
It is important to close the file after reading it
```

```py
f = open("file.txt", "r")    # 'r' or 'rt' is used to read text, use 'rb' to read binaries
content=f.read()
print(content)
f.close()
```
OR
```py
with open("file.txt", 'r') as f:
    content = f.read()
    print(content)
# no need to close the file if using 'with'
```
<img width="643" height="73" alt="image" src="https://github.com/user-attachments/assets/ce21c0da-977a-4c58-b56d-c90d868a0395" />

### Creating & writing to a file
```py
f = open("file2.txt", "w")
string = """This is a file we are creating from python.
This is where we can write to a file"""
f.write(string)
f.close()
```
`Output: A file named file2.txt will be created`

### Appending to a file 
```py
f = open("file2.txt", "a")
string = """
These are the additional lines I have added to the file.
I have used the append option to add additional text
"""
f.write(string)
f.close()
```
<img width="748" height="146" alt="image" src="https://github.com/user-attachments/assets/c7d7767a-0c6e-464f-9884-9121020ded23" />

#### Note:
- What if file doesn't exists:
  - read will throw an error
  - write & append will create a file

 ## WORKING WITH RELATED FILE MODULES
 ### OS Module
 ```py
import os
l = os.listdir("dir")
print(l)
```
<img width="197" height="200" alt="image" src="https://github.com/user-attachments/assets/d97d1260-5d77-42e9-b243-9a5ac85f5848" />
<img width="430" height="25" alt="image" src="https://github.com/user-attachments/assets/d09ca983-9744-4cd3-9530-8364df3fced4" />

