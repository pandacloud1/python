### FLASH MESSAGE
- Flash is a way to send a temporary message in browser.
- It is mainly used for: Login success message, Logout message, Error message, Form validation message
- Flash stores message temporarily in a session, then automatically removes it after reading
- Note: Flash requires a Secret Key, because flash stores data in session. Session is signed using secret key.So, No secret key → no flash.

#### main.py
```py
from flask import Flask, render_template, flash, redirect, url_for

app = Flask(__name__)

# The secret key protects your session data from being modified by users
# If there was no signature, user could edit cookie
app.secret_key = "random!secretkey!used!for!flash"

@app.route("/")
def index():
    return render_template("index.html")

@app.route("/logout")
def logout():
    flash("You have been logged out successfully!")
    return redirect(url_for("index"))

app.run(debug=True)
```
#### templates/index.html
```html
<!DOCTYPE html>
<html>
<head>
    <title>Home</title>
</head>
<body>

    <h2>Welcome to our Page!</h2>
    <a href="{{ url_for("logout") }}">Logout</a>

    <script>
        {% with messages = get_flashed_messages() %}
            {% if messages %}
                alert("{{ messages[0] }}")
            {% endif %}
        {% endwith %}
    </script>

</body>
</html>
```
<img width="412" height="231" alt="image" src="https://github.com/user-attachments/assets/d0237c5c-9525-41ad-8400-e74d14ef440f" />
<img width="1248" height="298" alt="image" src="https://github.com/user-attachments/assets/878fa0b9-e7c8-41c5-bbad-86646e9be72b" />

