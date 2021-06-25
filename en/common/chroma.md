---
layout: default
title: "chroma"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chroma">
  <a href="/en/common/chroma.html">chroma</a> <a href="#chroma"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Chroma is a general-purpose syntax highlighting library and corresponding command, for Go.
> More information: <https://github.com/alecthomas/chroma>.

#### Highlight a source file with python lexer and output to terminal:
```shell
chroma --lexer="{{python}}" {{source_file}}
```
#### Highlight a source file with Go lexer and output to a HTML file:
```shell
chroma --lexer="{{go}}" --formatter="{{html}}" {{source_file}} > {{html_file}}
```
#### Highlight a source file with C++ lexer and output to an SVG image, using the Monokai style:
```shell
chroma --lexer="{{c++}}" --formatter="{{svg}}" --syle="{{monokai}}" {{source_file}} > {{svg_file}}
```
{% endraw %}