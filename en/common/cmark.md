---
layout: default
title: "cmark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmark">
  <a href="/en/common/cmark.html">cmark</a> <a href="#cmark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts CommonMark Markdown formatted text to other formats.
> More information: <https://github.com/commonmark/cmark>.

#### Render a CommonMark Markdown file to HTML:
```shell
cmark --to html {{filename.md}}
```
#### Convert data from standard input to LaTeX:
```shell
cmark --to latex
```
#### Convert straight quotes to smart quotes:
```shell
cmark --smart --to html {{filename.md}}
```
#### Validate UTF-8 characters:
```shell
cmark --validate-utf8 {{filename.md}}
```
{% endraw %}