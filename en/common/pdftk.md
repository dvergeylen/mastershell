---
layout: default
title: "pdftk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftk">
  <a href="/en/common/pdftk.html">pdftk</a> <a href="#pdftk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PDF toolkit.
> More information: <https://www.pdflabs.com/tools/pdftk-the-pdf-toolkit>.

#### Extract pages 1-3, 5 and 6-10 from a PDF file and save them as another one:
```shell
pdftk {{input.pdf}} cat {{1-3 5 6-10}} output {{output.pdf}}
```
#### Merge (concatenate) a list of PDF files and save the result as another one:
```shell
pdftk {{file1.pdf file2.pdf ...}} cat output {{output.pdf}}
```
#### Split each page of a PDF file into a separate file, with a given filename output pattern:
```shell
pdftk {{input.pdf}} burst output {{out_%d.pdf}}
```
#### Rotate all pages by 180 degrees clockwise:
```shell
pdftk {{input.pdf}} cat {{1-endsouth}} output {{output.pdf}}
```
#### Rotate third page by 90 degrees clockwise and leave others unchanged:
```shell
pdftk {{input.pdf}} cat {{1-2 3east 4-end}} output {{output.pdf}}
```
{% endraw %}