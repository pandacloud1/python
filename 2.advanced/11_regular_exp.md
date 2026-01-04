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

### Find the number of occurences of a word
```py
# Let's print the number of occurences of the word 'the' (using 're.findall')
# Also use 're.IGNORECASE' to avoid case-sensitive search
import re
text = "The quick brown fox jumps over the lazy dog"

new_text = re.findall("the", text, re.IGNORECASE)
print (new_text) 
```
<img width="157" height="30" alt="image" src="https://github.com/user-attachments/assets/a3d2de9f-403e-41c9-801a-ba7fed806d3c" />

### Find and replace
```py
# Let's replace 'fox' with 'CAT' (using 're.sub')
import re
text = "The quick brown fox jumps over the lazy dog"

new_text = re.sub("fox", "CAT", text)
print (new_text)
```
<img width="493" height="22" alt="image" src="https://github.com/user-attachments/assets/0fa3af47-bb5b-4991-ae1a-3d5e7e811e2f" />
