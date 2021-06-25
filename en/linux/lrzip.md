---
layout: default
title: "lrzip"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lrzip">
  <a href="/en/linux/lrzip.html">lrzip</a> <a href="#lrzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A large file compression program.
> See also `lrunzip`, `lrztar`, `lrzuntar`.

#### Compress a file with LZMA - slow compression, fast decompression:
```shell
lrzip {{filename}}
```
#### Compress a file with BZIP2 - good middle ground for compression/speed:
```shell
lrzip -b {{filename}}
```
#### Compress with ZPAQ - extreme compression, but very slow:
```shell
lrzip -z {{filename}}
```
#### Compress with LZO - light compression, extremely fast decompression:
```shell
lrzip -l {{filename}}
```
#### Compress a file and password protect/encrypt it:
```shell
lrzip -e {{filename}}
```
#### Override the number of processor threads to use:
```shell
lrzip -p {{8}} {{filename}}
```
{% endraw %}