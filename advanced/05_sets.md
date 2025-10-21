## SETS
- They are unordered list of unique items
- They do not follow any order, hence you cannot print index of sets
- You can use set methods like add, remove, discard & pop
- Additionally, you can also use union, intersection & difference

### Set of fruits
```py
fruits = {"banana", "apple", "guava"}
print(fruits)
print(fruits[0])     # this is not possible
```
<img width="230" height="90" alt="image" src="https://github.com/user-attachments/assets/348d8f84-6c3f-4b4a-8bc7-608bb3225256" />

### Set functions
```py
set1 = {1,2,3,4,5}
set2 = {3,4,5,6,7}

union = set1.union(set2)
print(union)

intersect = set1.intersection(set2)
print(intersect)
```
<img width="145" height="51" alt="image" src="https://github.com/user-attachments/assets/4966647f-4d05-47b7-b2a0-926621a64fbe" />

diff = set1.difference(set2)
print(diff)
