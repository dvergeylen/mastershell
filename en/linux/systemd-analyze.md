---
layout: default
title: "systemd-analyze"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systemd-analyze">
  <a href="/en/linux/systemd-analyze.html">systemd-analyze</a> <a href="#systemd-analyze"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show timing details about the boot process of units (services, mount points, devices, sockets).

#### List time of each unit to start up:
```shell
systemd-analyze blame
```
#### Print a tree of the time critical chain of units:
```shell
systemd-analyze critical-chain
```
#### Create an SVG file showing when each system service started, highlighting the time that they spent on initialization:
```shell
systemd-analyze plot > {{path/to/file.svg}}
```
#### Plot a dependency graph and convert it to an SVG file:
```shell
systemd-analyze dot | dot -T{{svg}} > {{path/to/file.svg}}
```
{% endraw %}