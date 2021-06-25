---
layout: default
title: "mutool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mutool">
  <a href="/en/common/mutool.html">mutool</a> <a href="#mutool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert PDF files, query information and extract data.
> More information: <https://mupdf.com/docs>.

#### Convert pages 1-10 into 10 PNG images:
```shell
mutool convert -o {{image%d.png}} {{file.pdf}} {{1-10}}
```
#### Convert pages 2, 3 and 5 of a PDF into text in the standard output:
```shell
mutool draw -F {{txt}} {{file.pdf}} {{2,3,5}}
```
#### Concatenate two PDFs:
```shell
mutool merge -o {{output.pdf}} {{input1.pdf}} {{input2.pdf}}
```
#### Query information about all content embedded in a PDF:
```shell
mutool info {{input.pdf}}
```
#### Extract all images, fonts and resources embedded in a PDF out into the current directory:
```shell
mutool extract {{input.pdf}}
```
#### Print the outline (table of contents) of a PDF:
```shell
mutool show {{input.pdf}} outline
```
{% endraw %}