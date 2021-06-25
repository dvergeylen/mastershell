---
layout: default
title: "pdftotext"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftotext">
  <a href="/en/common/pdftotext.html">pdftotext</a> <a href="#pdftotext"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert PDF files to plain text format.

#### Convert `filename.pdf` to plain text and print it to standard output:
```shell
pdftotext {{filename.pdf}} -
```
#### Convert `filename.pdf` to plain text and save it as `filename.txt`:
```shell
pdftotext {{filename.pdf}}
```
#### Convert `filename.pdf` to plain text and preserve the layout:
```shell
pdftotext -layout {{filename.pdf}}
```
#### Convert `input.pdf` to plain text and save it as `output.txt`:
```shell
pdftotext {{input.pdf}} {{output.txt}}
```
#### Convert pages 2, 3 and 4 of `input.pdf` to plain text and save them as `output.txt`:
```shell
pdftotext -f {{2}} -l {{4}} {{input.pdf}} {{output.txt}}
```
{% endraw %}