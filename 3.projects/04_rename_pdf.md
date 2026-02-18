### Code to rename pdf files
```py
import os

i = 1
for file in os.listdir("."):                # "." means current directory
    if file.lower().endswith(".pdf"):
        os.rename(file, f"doc-{i}.pdf")
        i += 1

print("Done")
```
