---
layout: default
title: "pdfgrep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfgrep">
  <a href="/en/linux/pdfgrep.html">pdfgrep</a> <a href="#pdfgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search text in PDF files.

#### Find lines that match pattern in a PDF:
```shell
pdfgrep {{pattern}} {{file.pdf}}
```
#### Include file name and page number for each matched line:
```shell
pdfgrep --with-filename --page-number {{pattern}} {{file.pdf}}
```
#### Do a case insensitive search for lines that begin with "foo" and return the first 3 matches:
```shell
pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{file.pdf}}
```
#### Find pattern in files with a `.pdf` extension in the current directory recursively:
```shell
pdfgrep --recursive {{pattern}}
```
#### Find pattern on files that match a specific glob in the current directory recursively:
```shell
pdfgrep --recursive --include {{'*book.pdf'}} {{pattern}}
```
{% endraw %}