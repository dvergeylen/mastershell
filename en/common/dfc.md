---
layout: default
title: "dfc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dfc">
  <a href="/en/common/dfc.html">dfc</a> <a href="#dfc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gives an overview of the filesystem disk space usage with colours and graphs.
> More information: <https://projects.gw-computing.net/projects/dfc/wiki>.

#### Display filesystems and their disk usage in human readable form with colours and graphs:
```shell
dfc
```
#### Display all filesystems including pseudo, duplicate and inaccessible filesystems:
```shell
dfc -a
```
#### Display filesystems without colour:
```shell
dfc -c never
```
#### Display filesystems containing "ext" in the filesystem type:
```shell
dfc -t ext
```
{% endraw %}