---
layout: default
title: "latex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="latex">
  <a href="/en/common/latex.html">latex</a> <a href="#latex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile a DVI document from LaTeX source files.
> More information: <https://www.latex-project.org>.

#### Compile a DVI document:
```shell
latex {{source.tex}}
```
#### Compile a DVI document, specifying an output directory:
```shell
latex -output-directory={{path/to/directory}} {{source.tex}}
```
#### Compile a DVI document, halting on each error:
```shell
latex -halt-on-error {{source.tex}}
```
{% endraw %}