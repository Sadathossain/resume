# Resume
--------

This repo contains all my resume formats.

## Requirements
---------------

* [Pandoc](https://pandoc.org/)
* [Miktex](https://miktex.org/) for PDF generation with Windows
* [TinyTex](https://yihui.name/tinytex/) for PDF generation with MacOS

## Commands to generate different formats
-----------------------------------------

*  TXT
```bash
pandoc --standalone --from markdown+smart --to plain -o resume.txt resume.md
```

*  DOCX
```bash
pandoc --from markdown --to docx -o resume.docx resume.md
```

*  HTML
```bash
pandoc --standalone -c static/css/style.css --from markdown --to html -o resume.html resume.md
pandoc --standalone -c static/css/style.css --metadata pagetitle="Resume of Sadat Hossain" --from markdown --to html -o index.html resume.md
```

*  PDF
```bash
pandoc -s -o resume.pdf resume.md
```
