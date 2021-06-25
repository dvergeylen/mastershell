---
layout: default
title: "fold"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fold">
  <a href="/en/common/fold.html">fold</a> <a href="#fold"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wraps each line in an input file to fit a specified width and prints it to the standard output.
> More information: <https://www.gnu.org/software/coreutils/fold>.

#### Wrap each line to default width (80 characters):
```shell
fold {{file}}
```
#### Wrap each line to width "30":
```shell
fold -w30 {{file}}
```
#### Wrap each line to width "5" and break the line at spaces (puts each space separated word in a new line, words with length > 5 are wrapped):
```shell
fold -w5 -s {{file}}
```
{% endraw %}