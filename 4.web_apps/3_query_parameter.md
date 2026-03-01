### QUERY PARAMETERS
- A query parameter in Python refers to a way of passing additional information to a web server's URL.
- Eg. `www.example.com/?name=query_parameter`
- Without query parameters, the server wouldn’t know What you’re searching for or Which page number you want or Which filter you selected
- In the below example, we are passing it manually, but in real-time it is passed as per the user's input from the browser form
- When user types `laptop`, the browser automatically creates `https://amazon.com/search?product=laptop`
  ```
  <form action="/search" method="GET">
    <input type="text" name="product">
    <button type="submit">Search</button>
  </form>
  ```

#### main.py
```py
from flask import Flask, render_template, request
app = Flask(__name__)

@app.route("/", methods=["GET", "POST"])
def hello_world():
    name = "Panda"
    token = 2026
    if "name" in request.args.keys():
        name = request.args["name"]
    if "token" in request.args.keys():
        token = request.args["token"]
    return render_template("index.html", name=name, token=token)
app.run(debug=True)
```

#### /template/index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h1>Welcome {{name}}</h1>
    <h3>Your token number is {{token}}</h3>
</body>
</html>
```
<img width="408" height="256" alt="image" src="https://github.com/user-attachments/assets/9263e44d-2b35-4e00-9c31-7147627c9fd0" />
<img width="552" height="250" alt="image" src="https://github.com/user-attachments/assets/2bd2edb9-c531-4ab8-8a6b-2d97d9d0eb0e" />


