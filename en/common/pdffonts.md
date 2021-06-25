---
layout: default
title: "pdffonts"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdffonts">
  <a href="/en/common/pdffonts.html">pdffonts</a> <a href="#pdffonts"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable Document Format (PDF) file fonts information viewer.
> More information: <https://www.xpdfreader.com/pdffonts-man.html>.

#### Print PDF file fonts information:
```shell
pdffonts {{path/to/file.pdf}}
```
#### Specify user password for PDF file to bypass security restrictions:
```shell
pdffonts -upw {{password}} {{path/to/file.pdf}}
```
#### Specify owner password for PDF file to bypass security restrictions:
```shell
pdffonts -opw {{password}} {{path/to/file.pdf}}
```
#### Print additional information on location of the font that will be used when the PDF file is rasterized:
```shell
pdffonts -loc {{path/to/file.pdf}}
```
#### Print additional information on location of the font that will be used when the PDF file is converted to PostScript:
```shell
pdffonts -locPS {{path/to/file.pdf}}
```
{% endraw %}