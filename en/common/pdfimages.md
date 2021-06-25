---
layout: default
title: "pdfimages"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfimages">
  <a href="/en/common/pdfimages.html">pdfimages</a> <a href="#pdfimages"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for extracting images from PDFs.

#### Extract all images from a PDF file and save them as PNGs:
```shell
pdfimages -png {{path/to/file.pdf}} {{filename_prefix}}
```
#### Extract images from pages 3 to 5:
```shell
pdfimages -f {{3}} -l {{5}} {{path/to/file.pdf}} {{filename_prefix}}
```
#### Extract images from a PDF file and include the page number in the output filenames:
```shell
pdfimages -p {{path/to/file.pdf}} {{filename_prefix}}
```
#### List information about all the images in a PDF file:
```shell
pdfimages -list {{path/to/file.pdf}}
```
{% endraw %}