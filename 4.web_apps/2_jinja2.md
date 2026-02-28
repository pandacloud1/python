### JINJA2
- Jinja2 is a tool that allows Python to generate dynamic HTML pages.
- Jinja2 lets you:
  - Insert variables into HTML
  - Run loops
  - Use conditions
  - Create dynamic web pages

### WITHOUT JINJA2
- Let's print age
```py
# file name: main.py
from flask import Flask, render_template, request

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
    return render_template("index.html", age=age)
app.run(debug=True)
```

```html
# file name: /templates/index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    The age is as below:<br>
    Alexa is {{age['Alexa']}} years old.<br>
    Benji is {{age['Benji']}} years old.<br>
    Ethan is {{age['Ethan']}} years old.<br>
    Grace is {{age['Grace']}} years old.<br>
    Ilsa is {{age['Ilsa']}} years old.<br>
    Luther is {{age['Luther']}} years old.
</body>
</html>
```
<img width="188" height="190" alt="image" src="https://github.com/user-attachments/assets/24195b9d-6c80-4b54-8fd8-c9e8795274b3" />
