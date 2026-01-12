## Questions Game

```py
questions = [
    ["A. Which is the tallest building in the world?","1. Burj Khalifa", "2. Petronas Towers", "3. Eiffel Tower", "4. Taj Mahal", 1],
    ["B. Which is the largest planet in our solar system?","1. Mars", "2. Jupiter", "3. Earth", "4. Uranus", 2],
    ["C. Which is the largest continent?","1. America", "2. Africa", "3. Asia", "4. Europe", 3],
    ["D. Who invented the laws of motion?","1. Albert Einstein", "2. Charles Babbage", "3. Thomas Edison", "4. Isaac Newton", 4],
    ["E. How many bones are there in the human body?","1. 206", "2. 207", "3. 235", "4. 236", 1],
]

for q in questions:
    print(q[0]) 
    print(q[1], "\t", q[2])
    print(q[3], "\t", q[4])

    i = int(input("Select option: "))
    if (i==q[5]):
        print("Congrats, Correct answer!!")
        print()
    else:
        print("Sorry, you lost the game!")
        break
```
<img width="665" height="763" alt="image" src="https://github.com/user-attachments/assets/5d836079-b592-4924-9cb9-c46419c45dae" />
