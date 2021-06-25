---
layout: default
title: "md5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="md5">
  <a href="/en/osx/md5.html">md5</a> <a href="#md5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate MD5 cryptographic checksums.

#### Calculate the MD5 checksum for a file:
```shell
md5 {{filename}}
```
#### Calculate MD5 checksums for multiple files:
```shell
md5 {{filename1}} {{filename2}}
```
#### Output only the md5 checksum (no filename):
```shell
md5 -q {{filename}}
```
#### Print a checksum of the given string:
```shell
md5 -s {{string}}
```
{% endraw %}