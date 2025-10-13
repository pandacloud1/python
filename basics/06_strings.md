## STRINGS

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
print(name[5:])      # goes from 5th index character (or 6th letter) to last character 
print(name[0:10:2])  # keeps [(2-1=1] consecutive characters
print(name[0:10:3])  # keeps [(3-1)=2] consecutive characters
print(name[0:])      # considers last character
print(name[:])       # considers first & last character
print(name[:-1])     # skips the last character
# Note: Strings are immutable, you cannot replace string or index values
# name = "Panda"
# name[0] = "D"
# TypeError: 'str' object does not support item assignment
```
<img width="116" height="111" alt="image" src="https://github.com/user-attachments/assets/668913bb-1642-488f-9704-ec5a7f049730" />

### STRING METHODS
#### Cases
```py
name = "panda cloud"
print(len(name))
print(name.upper())
print(name.lower())
print(name.capitalize())  # Only first letter
print(name.title())       # First letter of each word
```
<img width="150" height="80" alt="image" src="https://github.com/user-attachments/assets/715ab8f0-dbeb-44ab-9908-fcce8e10c0b7" />

#### Whitespaces
```py
name = " Panda Cloud "
print(name.strip())    # removes whitespaces from left & right
print(name.lstrip())   # removes whitespace from left
print(name.rstrip())   # removes whitespace from right
```
<img width="131" height="50" alt="image" src="https://github.com/user-attachments/assets/26d394c0-8212-4216-8709-63d3c69ec676" />

#### Find & Replace
name = "Panda Cloud"
print(name.find("Panda"))                # index position of the word
print(name.replace("Cloud", "Academy"))  # Replace 'Cloud' --> 'Academy'
<img width="119" height="37" alt="image" src="https://github.com/user-attachments/assets/9b20d633-77d0-468b-8586-f1f52ce2fe0a" />
