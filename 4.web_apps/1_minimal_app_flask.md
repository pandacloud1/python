### A Minimal Application using Flask
- Flask is a lightweight web framework for Python that simplifies the process of building web applications and APIs
- It is used for building RESTful APIs and microservices.
- Also used for developing small to medium-sized web applications.
- This will simply create a normal "Hello World" app that can be accessed from local host

#### Run below command to install flask
```sh
pip install Flask
```

#### Copy the minimal application code & add `app.run(debug=True)`
```py
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello, World!</p>"

app.run(debug=True)
```

#### Access local host
- Open http://127.0.0.1:5000/ & you must be able to see 'Hello World'
<img width="321" height="163.5" alt="image" src="https://github.com/user-attachments/assets/d93c3fa2-196d-493e-9e81-d43edb26c017" />
