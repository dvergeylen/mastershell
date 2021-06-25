---
layout: default
title: "goreload"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="goreload">
  <a href="/en/common/goreload.html">goreload</a> <a href="#goreload"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Live reload utility for Go programs.
> More information: <https://github.com/acoshift/goreload>.

#### Set the name of the binary file to watch (defaults to `.goreload`):
```shell
goreload -b {{path/to/binary}} {{file}}.go
```
#### Set a custom log prefix (defaults to `goreload`):
```shell
goreload --logPrefix {{prefix}} {{file}}.go
```
#### Reload whenever any file changes:
```shell
goreload --all
```
{% endraw %}