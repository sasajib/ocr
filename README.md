ocr.sh: a bash script to OCR PDF files easily
=============================================

Author
------

Vincent Rasneur <vrasneur@free.fr>

Required programs
-----------------

* pdftk
* ghostscript
* imagemagick
* tesseract


Usage
-----

To OCR a PDF file

```bash
ocr.sh document.pdf
```

```bash
ocr.sh -t eng document.pdf
```

```bash
ocr.sh -t eng -c document.pdf
```


Output files
------------

For a PDF file named `doc1.pdf`, the script:

* creates a directory named `doc1`
* for each PDF page, a file named `pg_<number>.txt` is created inside this directory

Or, if the `-c` argument is used, the script:

* creates a directory named `doc1`
* creates a unique file named `doc1/doc1.txt`
