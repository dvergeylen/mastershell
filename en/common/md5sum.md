---
layout: default
title: "md5sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="md5sum">
  <a href="/en/common/md5sum.html">md5sum</a> <a href="#md5sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate MD5 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/md5sum>.

#### Calculate the MD5 checksum for a file:
```shell
md5sum {{filename1}}
```
#### Calculate MD5 checksums for multiple files:
```shell
md5sum {{filename1}} {{filename2}}
```
#### Read a file of MD5SUMs and verify all files have matching checksums:
```shell
md5sum -c {{filename.md5}}
```
#### Calculate a MD5 checksum from the standard input:
```shell
echo "{{text}}" | md5sum
```
{% endraw %}