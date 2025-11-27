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
 
### Counting number of lines in a file
```py
with open("file1.txt", "r") as f:
  lines = f.readlines()
  print(f"The number of lines are {len(lines)}")
```
<img width="293" height="30" alt="image" src="https://github.com/user-attachments/assets/a054a3e4-9f4d-490f-ad9c-4d86fda78f05" />

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

### sys module
```py
### Take file name & word & print number of times the word appears
import sys

def search_word(word, string):
    return string.count(word)

if __name__ == "__main__":
    filename = sys.argv[1]
    word = sys.argv[2]
    with open(filename) as f:
        string = f.read()
        n = search_word(word, string)
        print(n)
```
<img width="427" height="107" alt="image" src="https://github.com/user-attachments/assets/6c4cd451-31e7-4a20-be73-5b9b24c59013" />
<img width="507" height="47" alt="image" src="https://github.com/user-attachments/assets/38e16f85-43e5-4a35-804a-a2a5a61622c7" />


## COMMAND LINE UTILITIES
### Creating Command line utilities
```py
import argparse

parser = argparse.ArgumentParser(description = "Simple Calculator")

parser.add_argument("num1", type=float)
parser.add_argument("num2", type=float)
parser.add_argument("operation", choices=["add","sub","mul","div"])

args = parser.parse_args()

if(args.operation == "add"):
    print(f"The sum is {args.num1 + args.num2}")
elif(args.operation == "sub"):
    print(f"The difference is {args.num1 - args.num2}")
elif(args.operation == "mul"):
    print(f"The multiplication is {args.num1 * args.num2}")
elif(args.operation == "div"):
    print(f"The division is {args.num1 / args.num2}")
else:
    print("Error: Invalid input")

print(args)    # remove this line, if you do not want to print namespace 
```
<img width="522" height="308" alt="image" src="https://github.com/user-attachments/assets/56740ae6-b23e-4453-886b-1a8633381a85" />


