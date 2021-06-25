---
layout: default
title: "repquota"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="repquota">
  <a href="/en/linux/repquota.html">repquota</a> <a href="#repquota"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a summary of existing file quotas for a filesystem.

#### Report stats for all quotas in use:
```shell
sudo repquota -all
```
#### Report quota stats for all users, even those who aren't using any of their quota:
```shell
sudo repquota -v {{filesystem}}
```
#### Report on quotas for users only:
```shell
repquota --user {{filesystem}}
```
#### Report on quotas for groups only:
```shell
sudo repquota --group {{filesystem}}
```
#### Report on used quota and limits in a human-readable format:
```shell
sudo repquota --human-readable {{filesystem}}
```
#### Report on all quotas for users and groups in a human-readable format:
```shell
sudo repquota -augs
```
{% endraw %}