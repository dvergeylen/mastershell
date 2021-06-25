---
layout: default
title: "findmnt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="findmnt">
  <a href="/en/linux/findmnt.html">findmnt</a> <a href="#findmnt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find your filesystem.

#### List all mounted filesystems:
```shell
findmnt
```
#### Search for a device:
```shell
findmnt {{/dev/sdb1}}
```
#### Search for a mountpoint:
```shell
findmnt {{/}}
```
#### Find filesystems in specific type:
```shell
findmnt -t {{ext4}}
```
#### Find filesystems with specific label:
```shell
findmnt LABEL={{BigStorage}}
```
{% endraw %}