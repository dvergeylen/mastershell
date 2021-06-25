---
layout: default
title: "shred"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shred">
  <a href="/en/common/shred.html">shred</a> <a href="#shred"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Overwrite files to securely delete data.
> More information: <https://www.gnu.org/software/coreutils/shred>.

#### Overwrite a file:
```shell
shred {{file}}
```
#### Overwrite a file, leaving zeroes instead of random data:
```shell
shred --zero {{file}}
```
#### Overwrite a file 25 times:
```shell
shred -n25 {{file}}
```
#### Overwrite a file and remove it:
```shell
shred --remove {{file}}
```
{% endraw %}