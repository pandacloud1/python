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
 ### os module
 ```py
import os
print(os.listdir("dir"))
print(os.getcwd())            # checks current work dir
print(os.path.exists("dir"))  # check if file exists or not
os.remove("abcfile.txt")      # removes files
os.rmdir("abcdir")            # removes empty directories only
```
<img width="197" height="200" alt="image" src="https://github.com/user-attachments/assets/d97d1260-5d77-42e9-b243-9a5ac85f5848" />
<img width="431" height="77" alt="image" src="https://github.com/user-attachments/assets/94d2a393-4e64-4479-94aa-36b3988e7182" />

### shutil module
```py
import shutil 
import os
shutil.copy("test.py", "test.txt")
os.mkdir("dir")
os.mkdir("dir2")
shutil.move("test.txt", "dir/")
shutil.rmtree("dir2")
```
<img width="167" height="106" alt="image" src="https://github.com/user-attachments/assets/27f93a71-4960-4494-9f5e-eef4c6f5f20a" />

## COMMAND LINE UTILITIES
### Creating Command line utilities
```py
import argparse

parser = argparse.ArgumentParser(description = "Simple Calculator")
# ArgumentParser is a class from argparse module
# It allows your program to accept input from the terminal
# So instead of typing values inside the code, users can give inputs when running the script in terminal

parser.add_argument("num1", type=float, help="First_number")
parser.add_argument("num2", type=float, help="Second_number")
parser.add_argument("operation", choices=["add", "sub", "mult", "div"], help="Operation")

args = parser.parse_args()
# parse_args() reads the values that the user passes from the command line and stores them in an object (args).
print(args)

if(args.operation == "add"):
    print(f"The sum is {args.num1 + args.num2}")
elif(args.operation == "sub"):
    print(f"The difference is {args.num1 - args.num2}")
elif(args.operation == "mult"):
    print(f"The sum is {args.num1 * args.num2}")
elif(args.operation == "div"):
    print(f"The sum is {args.num1 / args.num2}")
else:
    print("Error: Invalid input")
```
<img width="565" height="307" alt="image" src="https://github.com/user-attachments/assets/c62b14b2-ecc3-4a39-9e72-1276133e86ba" />

