---
layout: default
title: "pigz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pigz">
  <a href="/en/common/pigz.html">pigz</a> <a href="#pigz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multithreaded zlib compression utility.
> More information: <https://github.com/madler/pigz>.

#### Compress a file with default options:
```shell
pigz {{filename}}
```
#### Compress a file using the best compression method:
```shell
pigz -9 {{filename}}
```
#### Compress a file using no compression and 4 processors:
```shell
pigz -0 -p{{4}} {{filename}}
```
#### Compress a directory using tar:
```shell
tar cf - {{path/to/directory}} | pigz > {{filename}}.tar.gz
```
#### Decompress a file:
```shell
pigz -d {{archive.gz}}
```
#### List the contents of an archive:
```shell
pigz -l {{archive.tar.gz}}
```
{% endraw %}