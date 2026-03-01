### CREATING API IN JSON FORMAT
- You can simply import `jsonify` to use json in python
- Right click in browser --> Inspect --> Network to verify if the document is json

#### main.py
```py
from flask import Flask, render_template, jsonify
app = Flask(__name__)

@app.route("/", methods=["GET", "POST"])
def hello_world():
    age = {
       "Alexa": 22,
       "Benji": 35,
       "Ethan": 53,
       "Grace": 45,       
       "Ilsa": 37,
       "Luther": 21
    }
    return jsonify(age)
app.run(debug=True)
```
<img width="1910" height="698" alt="image" src="https://github.com/user-attachments/assets/22bd96af-9377-49f1-b270-ef784a95a4dc" />
