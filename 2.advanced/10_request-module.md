## REQUESTS MODULE

- It is used to get data in form of text, json from URLs
- It simplifies the process of sending HTTP requests
- Used for making HTTP requests, Interacting with REST APIs, etc.
- You need to first install it using command `pip install requests`
- syntax --> `requests.get(url, params={key: value}, **kwargs)`

```py
import requests

r = requests.get("https://api.github.com/users/pandacloud1")
print(r.text)
```
<img width="740" height="139" alt="image" src="https://github.com/user-attachments/assets/08478b54-1516-4608-bd56-6c788c565325" />

```py
import requests

r = requests.get("https://api.github.com/users/pandacloud1")
with open("output.txt", "w") as f:
    f.write(r.text)
# you can also use
# requests.put, post, delete, head, options, etc
```
<img width="130" height="51" alt="image" src="https://github.com/user-attachments/assets/4e1dba47-fdcd-46f9-8c7a-4da068c979e0" />
