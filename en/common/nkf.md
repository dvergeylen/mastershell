---
layout: default
title: "nkf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nkf">
  <a href="/en/common/nkf.html">nkf</a> <a href="#nkf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Network kanji filter.
> Converts kanji code from one encoding to another.

#### Convert to UTF-8 encoding:
```shell
nkf -w {{path/to/file.txt}}
```
#### Convert to SHIFT_JIS encoding:
```shell
nkf -s {{path/to/file.txt}}
```
#### Convert to UTF-8 encoding and overwrite the file:
```shell
nkf -w --overwrite {{path/to/file.txt}}
```
#### Set new line code to LF and overwrite (unix type):
```shell
nkf -d --overwrite {{path/to/file.txt}}
```
#### Set new line code to CRLF and overwrite (windows type):
```shell
nkf -c --overwrite {{path/to/file.txt}}
```
#### Decrypt mime file and overwrite:
```shell
nkf -m --overwrite {{path/to/file.txt}}
```
{% endraw %}