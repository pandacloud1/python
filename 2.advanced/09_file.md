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
<img width="643" height="73" alt="image" src="https://github.com/user-attachments/assets/ce21c0da-977a-4c58-b56d-c90d868a0395" />
