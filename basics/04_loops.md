## LOOPS

### For loop (Print table of 5)
```py
for i in range (1, 11):    # [range is from 1 to (11-1) 10]
    print ("5 x", i, "=", (i)*5)
```
Output<br>
<img width="131" height="154" alt="image" src="https://github.com/user-attachments/assets/2b8b0f73-981b-452b-8bd3-4e75a08d00d8" />

### For loop (Print any multiplication table)
```py
n = int(input("Enter a number for multiplication table: "))

for i in range (1, 11):
    print (n, "x", i, "=", i*n)
```

### While loop (Print 1 to 5)
```py
i = 1
while i<6:
    print(i)  # 1 2 3 4 5 exit (Output)
    i+=1      # 2 3 4 5 6
```
