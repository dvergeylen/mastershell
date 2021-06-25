---
layout: default
title: "pandoc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pandoc">
  <a href="/en/common/pandoc.html">pandoc</a> <a href="#pandoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert documents between various formats.
> More information: <https://pandoc.org>.

#### Convert file to pdf (the output format is determined by file extension):
```shell
pandoc {{input.md}} -o {{output.pdf}}
```
#### Force conversion to use a specific format:
```shell
pandoc {{input.docx}} --to {{gfm}} -o {{output.md}}
```
#### Convert to a standalone file with the appropriate headers/footers (for LaTeX, HTML, etc.):
```shell
pandoc {{input.md}} -s -o {{output.tex}}
```
#### List all supported input formats:
```shell
pandoc --list-input-formats
```
#### List all supported output formats:
```shell
pandoc --list-output-formats
```
{% endraw %}