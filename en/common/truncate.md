---
layout: default
title: "truncate"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="truncate">
  <a href="/en/common/truncate.html">truncate</a> <a href="#truncate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shrink or extend the size of a file to the specified size.
> More information: <https://www.gnu.org/software/coreutils/truncate>.

#### Set a size of 10 GB to an existing file, or create a new file with the specified size:
```shell
truncate --size {{10G}} {{filename}}
```
#### Extend the file size by 50M, fill with holes (which reads as zero bytes):
```shell
truncate --size +{{50M}} {{filename}}
```
#### Shrink the file by 2GiB, by removing data from the end of file:
```shell
truncate --size -{{2G}} {{filename}}
```
#### Empty the file's content:
```shell
truncate --size 0 {{filename}}
```
#### Empty the file's content, but do not create the file if it does not exist:
```shell
truncate --no-create --size 0 {{filename}}
```
{% endraw %}