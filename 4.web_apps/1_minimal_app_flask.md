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

### Adding index.html files
- Now create two folders `static` & `templates` and your python code must be in `main.py`
- If you want to allow users to download files, then put those files inside `static` folder
- User can simple type the url, the path & download the files (eg. http://127.0.0.1:5000/static/hare.jpg)
- Go inside templates and add index.html file, just enter "!" and hit Enter, a template will be generated
- You can add your content there.
<img width="120" height="80" alt="image" src="https://github.com/user-attachments/assets/ca4cf497-f440-4c0e-ad0d-efaf1da21906" />

```py
### main.py
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def hello_world():
    return render_template("index.html")   # add index.html file name here

app.run(debug=True)   # default port is '5000', you can change it by entering port=x inside braces
                      # eg.: app.run(debug=True, port=8080)
```

```html
### Create index.html file inside 'templates'
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Welcome to the PandaCloud!</h1>
    <h3>Let's learn Python in simple way!</h3>
    
</body>
</html>
```
<img width="405" height="101" alt="image" src="https://github.com/user-attachments/assets/282e4e4a-bff7-4f3e-8474-638535c1f4bd" />

### Downloading content from app
- Add an image named 'img.jpg' inside `static` folder

```py
### main.py
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def hello_world():
    return render_template("index.html")

app.run(debug=True)
```
```html
### /templates/index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Welcome to the PandaCloud!</h1>
    <h3>Let's learn Python in simple way!</h3>
    <p>Download image here: </p><a href="/static/img.jpg">Download</a>
    
</body>
</html>
```
<img width="536" height="237" alt="image" src="https://github.com/user-attachments/assets/744f64aa-8e90-4ebe-9ef8-11b8e586b528" />
