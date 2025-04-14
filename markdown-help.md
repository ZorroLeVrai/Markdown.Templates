---
title: "Markdown Help"
---

# Markdown help

You can edit and view Markdown files using one of the following softwares
- VS Code
- MarkText
- StackEdit

Some extensions can be added to the Markdown software. But these extensions are not always compatible with other softwares.

If you want to generate *.docx, *.pdf or *.html files from your Markdown file, the best option is to use `pandoc`.

## Pandoc command lines

> Here is the command line to convert an *.md file into a *.docx file

```bash
pandoc your-document.md -o output.docx
```

Here is the command line to convert an *.md file into a *.pdf file

```bash
pandoc your-document.md -o output.pdf
```

> Please keep in mind that for .pdf files if your Markdown file contains some Latex formula, you will need to install as well `pdflatex` or `Miktex` (recommmended for Windows). So that `pandoc` knows how to convert these Latex notations into .pdf format.

Here is the command line to convert an *.md file into a *.html file

```bash
pandoc your-document.md -o output.html
```

If you want a stand-alone document you can add the `-s` option.

```bash
pandoc your-document.md -s -o output.html
```

If you want to embed all resources like images, you can add the `--embed-resources` option

```bash
pandoc your-document.md -s -o output.html --embed-resources
```
