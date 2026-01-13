## Merge pdf files together
- Install pypdf2 from web [https://pypi.org/project/PyPDF2/]
- Check documentation for pdf merge & run the code [https://pypdf2.readthedocs.io/en/3.x/user/merging-pdfs.html]

```py
from PyPDF2 import PdfWriter

merger = PdfWriter()

for pdf in ["pdf (1).pdf", "pdf (2).pdf", "pdf (3).pdf"]:
    merger.append(pdf)

merger.write("merged-pdf.pdf")
merger.close()
```
