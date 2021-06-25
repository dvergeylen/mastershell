---
layout: default
title: "pdfunite"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdfunite">
  <a href="/en/common/pdfunite.html">pdfunite</a> <a href="#pdfunite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PDF merging utility.
> More information: <https://github.com/mtgrosser/pdfunite>.

#### Merge 2 PDFs into a single PDF:
```shell
pdfunite {{path/to/fileA.pdf}} {{path/to/fileB.pdf}} {{path/to/merged_output.pdf}}
```
#### Merge a directory of PDFs into a single PDF:
```shell
pdfunite {{path/to/directory/*.pdf}} {{path/to/merged_output.pdf}}
```
{% endraw %}