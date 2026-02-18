### Code to rename only pdf files
```py
import os

i = 1
for file in os.listdir("."):                # "." means current directory
    if file.lower().endswith(".pdf"):
        os.rename(file, f"doc-{i}.pdf")
        i += 1

print("Done")
```

### Code to rename any files
```py
import os
prefix = input("Enter the file prefix: ")
ext = input("Enter the file extension: ")
i=1
for file in os.listdir("."):
    if file.endswith("." + ext):
        new_name = f"{prefix}-{i}.{ext}"
        os.rename (file, new_name)
        i+=1
```
<img width="347" height="56" alt="image" src="https://github.com/user-attachments/assets/4cc1d014-f96f-4b4b-8563-aeb470e43736" />
<img width="193" height="196" alt="image" src="https://github.com/user-attachments/assets/64043107-6a4d-4c6a-bda2-efbb629dfbbc" />

