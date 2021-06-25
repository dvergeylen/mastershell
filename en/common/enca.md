---
layout: default
title: "enca"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="enca">
  <a href="/en/common/enca.html">enca</a> <a href="#enca"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detect and convert the encoding of text files.
> More information: <https://github.com/nijel/enca>.

#### Detect file(s) encoding according to the system's locale:
```shell
enca {{file1 file2 ...}}
```
#### Detect file(s) encoding specifying a language in the POSIX/C locale format (e.g. zh_CN, en_US):
```shell
enca -L {{language}} {{file1 file2 ...}}
```
#### Convert file(s) to a specific encoding:
```shell
enca -L {{language}} -x {{to_encoding}} {{file1 file2 ...}}
```
#### Create a copy of an existing file using a different encoding:
```shell
enca -L {{language}} -x {{to_encoding}} < {{original_file}} > {{new_file}}
```
{% endraw %}