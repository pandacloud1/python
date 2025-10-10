## INDEX & STRING SLICING USED IN STRING

### INDEX
#### Print letters of a string in fwd/reverse order
```py
name = "PANDA"
print(name[0])
print(name[1])
print(name[2])
print(name[3])
print(name[4])
print()
print(name[-1])
print(name[-2])
print(name[-3])
print(name[-4])
print(name[-5])
```
<img width="146" height="172" alt="image" src="https://github.com/user-attachments/assets/eea9e8cb-ffec-4068-8a7a-c9872c530751" />

### STRING SLICING
#### Used to pick specific characters from a string
```py
name = "PANDACLOUD"  # word length = 10
print(name[0:5])     # goes from 0 to (5-1)
print(name[5:])      # goes from 5th character to last character
print(name[0:10:2])  # keeps [(2-1=1] consecutive characters
print(name[0:10:3])  # keeps [(3-1)=2] consecutive characters
print(name[0:])      # considers last character
print(name[:])       # considers first & last character
print(name[:-1])     # skips the last character
```
<img width="116" height="111" alt="image" src="https://github.com/user-attachments/assets/668913bb-1642-488f-9704-ec5a7f049730" />

