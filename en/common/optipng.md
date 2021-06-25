---
layout: default
title: "optipng"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="optipng">
  <a href="/en/common/optipng.html">optipng</a> <a href="#optipng"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PNG image file optimization utility.
> More information: <http://optipng.sourceforge.net>.

#### Compress a PNG with default settings:
```shell
optipng {{path/to/file.png}}
```
#### Compress a PNG with best compression:
```shell
optipng -o{{7}} {{path/to/file.png}}
```
#### Compress a PNG with fastest compression:
```shell
optipng -o{{0}} {{path/to/file.png}}
```
#### Compress a PNG and add interlacing:
```shell
optipng -i {{1}} {{path/to/file.png}}
```
#### Compress a PNG and preserve all metadata (including file timestamps):
```shell
optipng -preserve {{path/to/file.png}}
```
#### Compress a PNG and remove all metadata:
```shell
optipng -strip all {{path/to/file.png}}
```
{% endraw %}