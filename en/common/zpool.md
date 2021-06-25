---
layout: default
title: "zpool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zpool">
  <a href="/en/common/zpool.html">zpool</a> <a href="#zpool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage ZFS pools.

#### Show the configuration and status of all ZFS zpools:
```shell
zpool status
```
#### Check a ZFS pool for errors (verifies the checksum of EVERY block). Very CPU and disk intensive:
```shell
zpool scrub {{pool_name}}
```
#### List zpools available for import:
```shell
zpool import
```
#### Import a zpool:
```shell
zpool import {{pool_name}}
```
#### Export a zpool (unmount all filesystems):
```shell
zpool export {{pool_name}}
```
#### Show the history of all pool operations:
```shell
zpool history {{pool_name}}
```
#### Create a mirrored pool:
```shell
zpool create {{pool_name}} mirror {{disk1}} {{disk2}} mirror {{disk3}} {{disk4}}
```
#### Add a cache (L2ARC) device to a zpool:
```shell
zpool add {{pool_name}} cache {{cache_disk}}
```
{% endraw %}