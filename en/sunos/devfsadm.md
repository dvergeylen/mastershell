---
layout: default
title: "devfsadm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="devfsadm">
  <a href="/en/sunos/devfsadm.html">devfsadm</a> <a href="#devfsadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administration command for `/dev`. Maintains the `/dev` namespace.
> More information: <https://www.unix.com/man-page/sunos/1m/devfsadm>.

#### Scan for new disks:
```shell
devfsadm -c disk
```
#### Cleanup any dangling /dev links and scan for new device:
```shell
devfsadm -C -v
```
#### Dry-run - output what would be changed but make no modifications:
```shell
devfsadm -C -v -n
```
{% endraw %}