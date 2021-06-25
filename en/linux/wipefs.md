---
layout: default
title: "wipefs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wipefs">
  <a href="/en/linux/wipefs.html">wipefs</a> <a href="#wipefs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wipe filesystem, raid, or partition-table signatures from a device.

#### Display signatures for specified device:
```shell
sudo wipefs {{/dev/sdX}}
```
#### Wipe all available signatures for specified device:
```shell
sudo wipefs --all {{/dev/sdX}}
```
#### Perform dry run:
```shell
sudo wipefs --all --no-act {{/dev/sdX}}
```
#### Force wipe, even if the filesystem is mounted:
```shell
sudo wipefs --all --force {{/dev/sdX}}
```
{% endraw %}