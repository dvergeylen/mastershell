---
layout: default
title: "mupdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mupdf">
  <a href="/en/common/mupdf.html">mupdf</a> <a href="#mupdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MuPDF is a lightweight PDF, XPS, and E-book viewer.
> More information: <https://www.mupdf.com>.

#### Open a PDF on the first page:
```shell
mupdf {{filename}}
```
#### Open a PDF on page 3:
```shell
mupdf {{filename}} {{3}}
```
#### Open a password secured PDF:
```shell
mupdf -p {{password}} {{filename}}
```
#### Open a PDF with an initial zoom level, specified as DPI, of 72:
```shell
mupdf -r {{72}} {{filename}}
```
#### Open a PDF with inverted color:
```shell
mupdf -I {{filename}}
```
#### Open a PDF tinted red #FF0000 (hexadecimal color syntax RRGGBB):
```shell
mupdf -C {{FF0000}}
```
#### Open a PDF without anti-aliasing (0 = off, 8 = best):
```shell
mupdf -A {{0}}
```
{% endraw %}