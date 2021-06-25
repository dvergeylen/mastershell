---
layout: default
title: "ect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ect">
  <a href="/en/common/ect.html">ect</a> <a href="#ect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Efficient Compression Tool.
> File optimizer written in C++. It supports `.png`, `.jpg`, `.gzip` and `.zip` files.
> More information: <https://github.com/fhanau/Efficient-Compression-Tool>.

#### Compress a file:
```shell
ect {{path/to/file.png}}
```
#### Compress a file with specified compression level and multithreading (1=Fastest (Worst), 9=Slowest (Best), default is 3):
```shell
ect -{{9}} --mt-deflate {{path/to/file.zip}}
```
#### Compress all files in a directory recursively:
```shell
ect -recurse {{path/to/directory}}
```
#### Compress a file, keeping the original modification time:
```shell
ect -keep {{path/to/file.png}}
```
#### Compress a file, stripping metadata:
```shell
ect -strip {{path/to/file.png}}
```
{% endraw %}