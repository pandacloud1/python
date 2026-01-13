## Merge PDF
- Install pypdf2 from web [https://pypi.org/project/PyPDF2/]
- Check documentation for pdf merge & run the code [https://pypdf2.readthedocs.io/en/3.x/user/merging-pdfs.html]

### Direct merge
```py
from PyPDF2 import PdfWriter

merger = PdfWriter()

for pdf in ["pdf (1).pdf", "pdf (2).pdf", "pdf (3).pdf"]:
    merger.append(pdf)

merger.write("merged-pdf.pdf")
merger.close()
```

### Merge as per user's input
```py
from PyPDF2 import PdfWriter

merger = PdfWriter()

pdfs = []
n = int(input("Enter the number of files to merge: "))

for i in range(0, n):
    name = input(f"Enter the name of pdf {i+1}: ")
    pdfs.append(name)

for pdf in pdfs:
    merger.append(pdf)

merger.write("merged-pdf.pdf")
merger.close()
```
