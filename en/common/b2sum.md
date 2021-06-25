---
layout: default
title: "b2sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="b2sum">
  <a href="/en/common/b2sum.html">b2sum</a> <a href="#b2sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate BLAKE2 cryptographic checksums.
> More information: <https://www.gnu.org/software/coreutils/b2sum>.

#### Calculate the BLAKE2 checksum for a file:
```shell
b2sum {{filename1}}
```
#### Calculate BLAKE2 checksums for multiple files:
```shell
b2sum {{filename1}} {{filename2}}
```
#### Read a file of BLAKE2 sums and filenames and verify all files have matching checksums:
```shell
b2sum -c {{filename.b2}}
```
#### Calculate the BLAKE2 checksum from stdin:
```shell
{{somecommand}} | b2sum
```
{% endraw %}