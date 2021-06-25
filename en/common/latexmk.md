---
layout: default
title: "latexmk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="latexmk">
  <a href="/en/common/latexmk.html">latexmk</a> <a href="#latexmk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile LaTeX source files into finished documents.
> Automatically does multiple runs when needed.
> More information: <https://mg.readthedocs.io/latexmk.html>.

#### Compile a DVI (Device Independent file) document from every source:
```shell
latexmk
```
#### Compile a DVI document from a specific source file:
```shell
latexmk {{source.tex}}
```
#### Compile a pdf document:
```shell
latexmk -pdf {{source.tex}}
```
#### Force the generation of a document even if there are errors:
```shell
latexmk -f {{source.tex}}
```
#### Clean up temporary tex files created for a specific tex file:
```shell
latexmk -c {{source.tex}}
```
#### Clean up all temporary tex files in the current directory:
```shell
latexmk -c
```
{% endraw %}