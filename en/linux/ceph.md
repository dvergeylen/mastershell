---
layout: default
title: "ceph"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ceph">
  <a href="/en/linux/ceph.html">ceph</a> <a href="#ceph"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A unified storage system.
> More information: <https://ceph.io>.

#### Check cluster health status:
```shell
ceph status
```
#### Check cluster usage stats:
```shell
ceph df
```
#### Get the statistics for the placement groups in a cluster:
```shell
ceph pg dump --format {{plain}}
```
#### Create a storage pool:
```shell
ceph osd pool create {{pool_name}} {{page_number}}
```
#### Delete a storage pool:
```shell
ceph osd pool delete {{pool_name}}
```
#### Rename a storage pool:
```shell
ceph osd pool rename {{current_name}} {{new_name}}
```
#### Self-repair pool storage:
```shell
ceph pg repair {{pool_name}}
```
{% endraw %}