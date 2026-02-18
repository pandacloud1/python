### GENERATE QRCODE FROM URL

Ref: [https://pypi.org/project/qrcode/]
#### Install qrcode module using below commands
```pip install qrcode```
```pip install qrcode[pil]```

```py
import qrcode

url = input("Enter the url: ")
name = input("Enter the qrcode image name: ")

img = qrcode.make(url)
img.save(f"{name}.png")
```
