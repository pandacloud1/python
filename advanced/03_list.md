## LIST
- Lists are ordered & mutuable list of elements
- You can insert, delete or update elements

### Simple list example
```py
marks = [45,67,93,75,82]
print(marks)          # print all
print(marks[2:4])     # print index range

mixed = ["Mumbai", 2, True, 2.2, "Maharashtra"]
print(mixed)                                  # print all
print(f"The city name is {mixed[0]}")         # print specific index
print(f"The national rank is {mixed[1]}")     # print specific index
print(f"Is it a capital city? {mixed[2]}")    # print specific index
print(f"The population is {mixed[3]} crore")  # print specific index
```
<img width="269" height="112" alt="image" src="https://github.com/user-attachments/assets/3c6dda7a-f0a8-46c7-a354-5f8a25d06e87" />

### Changing the list
```py
# Lists are mutuable, below is an example
# This doesn't work with string
marks = [45,67,93,75,82]
print(marks)         # print all
marks[0] = 51
marks[1] = 70
marks[2] = 95
marks[3] = 82
marks[4] = 87
print(marks)         # print the changed list
```
<img width="139" height="35" alt="image" src="https://github.com/user-attachments/assets/98ccee8a-28d6-4f88-bdcc-30d6a20a6e30" />

### List methods (Paris)
```py
fruits = ['Apple','Banana','Cherry','Dates','Figs']

fruits.pop()                     # pop out last item
print (fruits)

fruits.append('Guava')           # append: add something at the end
print (fruits)

fruits.reverse()                 # reverse items in the list
print (fruits)

fruits.insert(1, 'Dragonfruit')  # insert at specific index (eg. 1)
print (fruits)

fruits.sort()                    # sort the items
print (fruits)

fruits.remove('Guava')           # remove specific item
print (fruits)
```
<img width="412" height="97" alt="image" src="https://github.com/user-attachments/assets/c2d91381-5304-4823-87ae-9b4ba33c371f" />
