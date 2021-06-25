---
layout: default
title: "virsh pool-delete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-delete">
  <a href="/en/common/virsh-pool-delete.html">virsh pool-delete</a> <a href="#virsh-pool-delete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete the underlying storage system of an inactive virtual machine storage pool.
> See also: `virsh`, `virsh-pool-destroy`, `virsh-pool-undefine`.
> More information: <https://manned.org/virsh>.

#### Delete the underlying storage system for the storage pool specified by name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-delete --pool {{name|uuid}}
```
{% endraw %}