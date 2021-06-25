---
layout: default
title: "findfs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="findfs">
  <a href="/en/linux/findfs.html">findfs</a> <a href="#findfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds a filesystem by label or UUID.
> More information: <https://mirrors.edge.kernel.org/pub/linux/utils/util-linux>.

#### Search block devices by filesystem label:
```shell
findfs LABEL={{label}}
```
#### Search by filesystem UUID:
```shell
findfs UUID={{uuid}}
```
#### Search by partition label (GPT or MAC partition table):
```shell
findfs PARTLABEL={{partition_label}}
```
#### Search by partition UUID (GPT partition table only):
```shell
findfs PARTUUID={{partition_uuid}}
```
{% endraw %}