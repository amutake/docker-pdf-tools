# pdf-tools

A Dockerfile containing various pdf-related tools

## tools

- pdftk
- imagemagick
- exiftool
- pdffonts

## how to use

```
host> ls
main.pdf
host> docker run -it --rm -v $(pwd):/workdir amutake/pdf-tools /bin/bash
container> pdffonts main.pdf
name                                 type              encoding         emb sub uni object ID
------------------------------------ ----------------- ---------------- --- --- --- ---------
ZIPAMY+IPAGothic                     CID TrueType      Identity-H       yes yes yes      9  0
HJIZJS+IPAMincho                     CID TrueType      Identity-H       yes yes yes     12  0
VACQAE+SFBX1000                      Type 1C           MacRoman         yes yes no       8  0
PJMMBA+SFSS1000                      Type 1C           MacRoman         yes yes no      10  0
XKROLA+SFRM1000                      Type 1C           MacRoman         yes yes no      11  0
...
```
