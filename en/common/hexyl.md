---
layout: default
title: "hexyl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="hexyl">
  <a href="/en/common/hexyl.html">hexyl</a> <a href="#hexyl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple hex viewer for the terminal. Uses colored output to distinguish different categories of bytes.
> More information: <https://github.com/sharkdp/hexyl>.

#### Print the hexadecimal representation of a file:
```shell
hexyl {{path/to/file}}
```
#### Print the hexadecimal representation of the first n bytes of a file:
```shell
hexyl -n {{n}} {{path/to/file}}
```
#### Print bytes 512 through 1024 of a file:
```shell
hexyl -r {{512}}:{{1024}} {{path/to/file}}
```
#### Print 512 bytes starting at the 1024th byte:
```shell
hexyl -r {{1024}}:+{{512}} {{path/to/file}}
```
{% endraw %}