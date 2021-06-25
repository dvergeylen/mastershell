---
layout: default
title: "fstrim"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fstrim">
  <a href="/en/linux/fstrim.html">fstrim</a> <a href="#fstrim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Discard unused blocks on a mounted filesystem.
> Only supported by flash memory devices such as SSDs and microSD cards.

#### Trim unused blocks on all mounted partitions that support it:
```shell
sudo fstrim --all
```
#### Trim unused blocks on a specified partition:
```shell
sudo fstrim {{/}}
```
#### Display statistics after trimming:
```shell
sudo fstrim --verbose {{/}}
```
{% endraw %}