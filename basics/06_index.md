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

### SLICING
#### Used to pick specific characters from a string
```py
name = "PANDACLOUD"  # word length = 10
print(name[0:5])     # goes from 0 to (5-1)
print(name[0:10:2])  # skips [(2-1=1] consecutive characters
print(name[0:10:3])  # skips [(3-1)=2] consecutive characters
print(name[0:])      # considers last character if not defined
print(name[:])       # considers first to last characters if not defined
print(name[:-1])     # skips the last character
```
<img width="154" height="94" alt="image" src="https://github.com/user-attachments/assets/bfdbbfa3-c8ef-4e01-a958-565bfcc9f41c" />
