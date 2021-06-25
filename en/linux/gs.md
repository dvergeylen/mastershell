---
layout: default
title: "gs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gs">
  <a href="/en/linux/gs.html">gs</a> <a href="#gs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GhostScript is a PDF and PostScript interpreter.

#### To view a file:
```shell
gs -dQUIET -dBATCH {{file.pdf}}
```
#### Reduce PDF file size to 150 dpi images for reading on a e-book device:
```shell
gs -dNOPAUSE -dQUIET -dBATCH -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook -sOutputFile={{output.pdf}} {{input.pdf}}
```
#### Convert PDF file (pages 1 through 3) to an image with 150 dpi resolution:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=jpeg -r150 -dFirstPage={{1}} -dLastPage={{3}} -sOutputFile={{output_%d.jpg}} {{input.pdf}}
```
#### Extract pages from a PDF file:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.pdf}}
```
#### Merge PDF files:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input1.pdf}} {{input2.pdf}}
```
#### Convert from PostScript file to PDF file:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.ps}}
```
{% endraw %}