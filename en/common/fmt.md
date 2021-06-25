---
layout: default
title: "fmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fmt">
  <a href="/en/common/fmt.html">fmt</a> <a href="#fmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reformat a text file by joining its paragraphs and limiting the line width to given number of characters (75 by default).
> More information: <https://www.gnu.org/software/coreutils/fmt>.

#### Reformat a file:
```shell
fmt {{path/to/file}}
```
#### Reformat a file producing output lines of (at most) `n` characters:
```shell
fmt -w {{n}} {{path/to/file}}
```
#### Reformat a file without joining lines shorter than the given width together:
```shell
fmt -s {{path/to/file}}
```
#### Reformat a file with uniform spacing (1 space between words and 2 spaces between paragraphs):
```shell
fmt -u {{path/to/file}}
```
{% endraw %}