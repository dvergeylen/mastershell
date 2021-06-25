---
layout: default
title: "pdflatex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdflatex">
  <a href="/en/common/pdflatex.html">pdflatex</a> <a href="#pdflatex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a PDF document from LaTeX source files.
> More information: <https://manned.org/pdflatex>.

#### Compile a PDF document:
```shell
pdflatex {{source.tex}}
```
#### Compile a PDF document specifying an output directory:
```shell
pdflatex -output-directory={{path/to/directory}} {{source.tex}}
```
#### Compile a PDF document, halting on each error:
```shell
pdflatex -halt-on-error {{source.tex}}
```
{% endraw %}