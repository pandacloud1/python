## TUPLES
- Tuples are same as list
- But they cannot be altered (immutable)
- They are written inside round braces()
- You can add a single entry in list, but in tuples you need to add additional comma [eg. name = ("Panda",)]
- Unlike list methods, tuples do not have any tuple methods

### Tuple example
```py
tup = ("Panda", "Cloud", "Academy")
print(tup)

# Tuples are immutable
tup[2] = "Institute"
print(tup)
```
<img width="390" height="110" alt="image" src="https://github.com/user-attachments/assets/f89365e4-cbc7-4722-a198-bea28d3804cb" />

### Tuple variable assign
```py
# We can assign variables to tuple items
tup = (2,3,4)
a,b,c = tup
print(a,b,c)
```
<img width="47" height="17" alt="image" src="https://github.com/user-attachments/assets/91046718-64e4-4e76-86ab-a70b140996da" />

### Tuple count & index
```py
tup = (2,3,4,2,5)
print(tup.count(2))
print(tup.index(2))
```
<img width="40" height="33" alt="image" src="https://github.com/user-attachments/assets/42ea871d-aae8-4f51-9d5c-dd490899d7de" />

