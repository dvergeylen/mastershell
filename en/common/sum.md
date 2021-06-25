---
layout: default
title: "sum"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sum">
  <a href="/en/common/sum.html">sum</a> <a href="#sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compute checksums and the number of blocks for a file.
> A predecessor to the more modern `cksum`.
> More information: <https://www.gnu.org/software/coreutils/sum>.

#### Compute a checksum with BSD-compatible algorithm and 1024-byte blocks:
```shell
sum {{file}}
```
#### Compute a checksum with System V-compatible algorithm and 512-byte blocks:
```shell
sum --sysv {{file}}
```
{% endraw %}