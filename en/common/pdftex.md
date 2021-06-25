---
layout: default
title: "pdftex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pdftex">
  <a href="/en/common/pdftex.html">pdftex</a> <a href="#pdftex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a PDF document from TeX source files.
> More information: <https://www.tug.org/applications/pdftex/>.

#### Compile a PDF document:
```shell
pdftex {{source.tex}}
```
#### Compile a PDF document, specifying an output directory:
```shell
pdftex -output-directory={{path/to/directory}} {{source.tex}}
```
#### Compile a PDF document, halting on each error:
```shell
pdftex -halt-on-error {{source.tex}}
```
{% endraw %}