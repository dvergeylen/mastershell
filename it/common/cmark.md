---
layout: default
title: "cmark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmark">
  <a href="/it/common/cmark.html">cmark</a> <a href="#cmark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converte testo CommonMark Markdown in altri formati.
> Maggiori informazioni: <https://github.com/commonmark/cmark>.

#### Converti un file Markdown in HTML:
```shell
cmark --to html {{file.md}}
```
#### Converti in LaTeX da standard input:
```shell
cmark --to latex
```
#### Converti apici semplici in apici intelligenti:
```shell
cmark --smart --to html {{file.md}}
```
#### Converti validando i caratteri UTF-8:
```shell
cmark --validate-utf8 {{file.md}}
```
{% endraw %}