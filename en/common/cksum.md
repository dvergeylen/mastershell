---
layout: default
title: "cksum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cksum">
  <a href="/en/common/cksum.html">cksum</a> <a href="#cksum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculates CRC checksums and byte counts of a file.
> Note, on old UNIX systems the CRC implementation may differ.
> More information: <https://www.gnu.org/software/coreutils/cksum>.

#### Display a 32 bit checksum, size in bytes and filename:
```shell
cksum {{filename}}
```
{% endraw %}