---
layout: default
title: "partprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="partprobe">
  <a href="/en/linux/partprobe.html">partprobe</a> <a href="#partprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Notify the operating system kernel of partition table changes.
> More information: <https://manned.org/partprobe>.

#### Notify the operating system kernel of partition table changes:
```shell
sudo partprobe
```
#### Notify the kernel of partition table changes and show a summary of devices and their partitions:
```shell
sudo partprobe --summary
```
#### Show a summary of devices and their partitions but don't notify the kernel:
```shell
sudo partprobe --summary --dry-run
```
{% endraw %}