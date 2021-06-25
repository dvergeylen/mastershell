---
layout: default
title: "pdftocairo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftocairo">
  <a href="/en/common/pdftocairo.html">pdftocairo</a> <a href="#pdftocairo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts PDF files to PNG/JPEG/TIFF/PDF/PS/EPS/SVG using cairo.
> More information: <https://poppler.freedesktop.org>.

#### Convert a PDF file to JPEG:
```shell
pdftocairo {{path/to/file.pdf}} -jpeg
```
#### Convert to PDF expanding the output to fill the paper:
```shell
pdftocairo {{path/to/file.pdf}} {{output.pdf}} -pdf -expand
```
#### Convert to SVG specifying the first/last page to convert:
```shell
pdftocairo {{path/to/file.pdf}} {{output.svg}} -svg -f {{first_page}} -l {{last_page}}
```
#### Convert to PNG with 200ppi resolution:
```shell
pdftocairo {{path/to/file.pdf}} {{output.png}} -png -r 200
```
#### Convert to grayscale TIFF setting paper size to A3:
```shell
pdftocairo {{path/to/file.pdf}} -tiff -gray -paper A3
```
#### Convert to PNG cropping x and y pixels from the top left corner:
```shell
pdftocairo {{path/to/file.pdf}} -png -x {{x_pixels}} -y {{y_pixels}}
```
{% endraw %}