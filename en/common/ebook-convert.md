---
layout: default
title: "ebook-convert"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ebook-convert">
  <a href="/en/common/ebook-convert.html">ebook-convert</a> <a href="#ebook-convert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Can be used to convert e-books between common formats, e.g., pdf, epub and mobi.
> Part of the Calibre e-book library tool.
> More information: <https://manual.calibre-ebook.com/generated/en/ebook-convert.html>.

#### Convert an e-book into another format:
```shell
ebook-convert {{source}} {{destination}}
```
#### Convert Markdown or HTML to e-book with TOC, title and author:
```shell
ebook-convert {{source}} {{destination}} --level1-toc="//h:h1" --level2-toc="//h:h2" --level3-toc="//h:h3" --title={{title}} --authors={{author}}
```
{% endraw %}