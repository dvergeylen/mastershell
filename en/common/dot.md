---
layout: default
title: "dot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dot">
  <a href="/en/common/dot.html">dot</a> <a href="#dot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool to produce layered drawings of directed graphs.
> More information: <https://www.graphviz.org/pdf/dotguide.pdf>.

#### Render an image file and determine output filename based on input filename and selected format:
```shell
dot -Tpng -O {{path/to/file.dot}}
```
#### Create an SVG from DOT file:
```shell
dot -Tsvg -o {{path/to/out_file.svg}} {{path/to/file.dot}}
```
{% endraw %}