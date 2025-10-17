## LIST
- Lists are ordered & mutuable list of elements
- You can insert, delete or update elements

### Simple list example
```py
marks = [45,67,93,75,82]
print(marks)          # print all
print(marks[2:4])     # print index range

mixed = ["Mumbai", 2, True, 2.2, "Maharashtra"]
print(mixed)          # print all
print(mixed[0])       # print specific index
```
<img width="267" height="65" alt="image" src="https://github.com/user-attachments/assets/8101fba0-21fa-4858-9fa9-f37352e4aeaa" />

### Changing the list
```py
# Lists are mutuable, below is an example
# This doesn't works with string
marks = [45,67,93,75,82]
print(marks)          # print all
marks[0] = 51
marks[1] = 70
marks[2] = 95
marks[3] = 82
marks[4] = 87
print(marks)         # print the changed list
```
<img width="139" height="35" alt="image" src="https://github.com/user-attachments/assets/98ccee8a-28d6-4f88-bdcc-30d6a20a6e30" />
