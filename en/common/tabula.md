---
layout: default
title: "tabula"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tabula">
  <a href="/en/common/tabula.html">tabula</a> <a href="#tabula"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract tables from PDF files.
> More information: <https://tabula.technology>.

#### Extract all tables from a PDF to a CSV file:
```shell
tabula -o {{file.csv}} {{file.pdf}}
```
#### Extract all tables from a PDF to a JSON file:
```shell
tabula --format JSON -o {{file.json}} {{file.pdf}}
```
#### Extract tables from pages 1, 2, 3, and 6 of a PDF:
```shell
tabula --pages {{1-3,6}} {{file.pdf}}
```
#### Extract tables from page 1 of a PDF, guessing which portion of the page to examine:
```shell
tabula --guess --pages {{1}} {{file.pdf}}
```
#### Extract all tables from a PDF, using ruling lines to determine cell boundaries:
```shell
tabula --spreadsheet {{file.pdf}}
```
#### Extract all tables from a PDF, using blank space to determine cell boundaries:
```shell
tabula --no-spreadsheet {{file.pdf}}
```
{% endraw %}