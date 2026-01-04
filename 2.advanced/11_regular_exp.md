## REGULAR EXPRESSION MODULE

- It is used for pattern searching (eg. search word index)
- Also used to modify the data (eg. find and replace a word from a string)

### Find the word's index position
```py
# Let's search the index for the word 'brown'
import re
text = "The quick brown fox jumps over the lazy dog"

result = re.search("brown", text)
print (result)
# In the output, 10 means that start of the index & 15 means end of the index
```
<img width="1106" height="55" alt="image" src="https://github.com/user-attachments/assets/335471f3-d830-4d37-94be-bb05d67780e7" />

<img width="461" height="93" alt="image" src="https://github.com/user-attachments/assets/fc82fd52-501c-4fb2-bd41-6979556c8db3" />

### We will print the same program, but with index output
```py
import re
text = "The quick brown fox jumps over the lazy dog"

result = re.search("brown", text)
print (result) 

if result:
    print("Match found!")
    print("Start index:", result.start())
    print("End index:", result.end())
```
<img width="546" height="107" alt="image" src="https://github.com/user-attachments/assets/2137a5a5-0786-43f1-bc8e-caed279ab588" />

