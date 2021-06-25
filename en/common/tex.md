---
layout: default
title: "tex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tex">
  <a href="/en/common/tex.html">tex</a> <a href="#tex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a DVI document from TeX source files.
> More information: <https://www.tug.org/begin.html>.

#### Compile a DVI document:
```shell
tex {{source.tex}}
```
#### Compile a DVI document, specifying an output directory:
```shell
tex -output-directory={{path/to/directory}} {{source.tex}}
```
#### Compile a DVI document, halting on each error:
```shell
tex -halt-on-error {{source.tex}}
```
{% endraw %}