---
layout: default
title: "cfdisk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cfdisk">
  <a href="/en/linux/cfdisk.html">cfdisk</a> <a href="#cfdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A program for managing partition tables and partitions on a hard disk using a curses UI.
> More information: <https://manned.org/cfdisk>.

#### Start the partition manipulator with a specific device:
```shell
cfdisk {{/dev/sdX}}
```
#### Create a new partition table for a specific device and manage it:
```shell
cfdisk --zero {{/dev/sdX}}
```
{% endraw %}