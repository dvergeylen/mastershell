---
layout: default
title: "lzop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lzop">
  <a href="/en/common/lzop.html">lzop</a> <a href="#lzop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compress or decompress files with LZO compression.
> More information: <https://www.lzop.org/>.

#### Compress a file into a new file with the `.lzo` suffix:
```shell
lzop {{file}}
```
#### Decompress a file:
```shell
lzop -d {{file}}.lzo
```
#### Compress a file, while specifying the compression level. 0 = Worst, 9 = Best (Default level is 3):
```shell
lzop -{{level}} {{file}}
```
{% endraw %}