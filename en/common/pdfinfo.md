---
layout: default
title: "pdfinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfinfo">
  <a href="/en/common/pdfinfo.html">pdfinfo</a> <a href="#pdfinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable Document Format (PDF) file information viewer.
> More information: <https://www.xpdfreader.com/pdfinfo-man.html>.

#### Print PDF file information:
```shell
pdfinfo {{path/to/file.pdf}}
```
#### Specify user password for PDF file to bypass security restrictions:
```shell
pdfinfo -upw {{password}} {{path/to/file.pdf}}
```
#### Specify owner password for PDF file to bypass security restrictions:
```shell
pdfinfo -opw {{password}} {{path/to/file.pdf}}
```
{% endraw %}