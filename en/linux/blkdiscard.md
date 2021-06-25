---
layout: default
title: "blkdiscard"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="blkdiscard">
  <a href="/en/linux/blkdiscard.html">blkdiscard</a> <a href="#blkdiscard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Discards device sectors on storage devices. Useful for SSDs.

#### Discard all sectors on a device, removing all data:
```shell
blkdiscard /dev/{{device}}
```
#### Securely discard all blocks on a device, removing all data:
```shell
blkdiscard --secure /dev/{{device}}
```
#### Discard the first 100MB of a device:
```shell
blkdiscard --length {{100MB}} /dev/{{device}}
```
{% endraw %}