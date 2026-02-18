### GENERATE QRCODE FROM URL

Ref: [https://pypi.org/project/qrcode/]
#### Install qrcode module using below commands
```txt
pip install qrcode
```
```txt
pip install qrcode[pil]
```

```py
import qrcode

url = input("Enter the url: ")
name = input("Enter the qrcode image name: ")

img = qrcode.make(url)
img.save(f"{name}.png")
```
<img width="376" height="373" alt="image" src="https://github.com/user-attachments/assets/b7912852-c297-4a98-8581-a9f02586f0be" />
