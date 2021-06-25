---
layout: default
title: "virsh pool-info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-info">
  <a href="/en/common/virsh-pool-info.html">virsh pool-info</a> <a href="#virsh-pool-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about a virtual machine storage pool.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### List the name, UUID, state, persistence type, autostart status, capacity, space allocated, and space available for the storage pool specified by name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-info --pool {{name|uuid}}
```
{% endraw %}