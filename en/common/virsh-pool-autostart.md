---
layout: default
title: "virsh pool-autostart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-autostart">
  <a href="/en/common/virsh-pool-autostart.html">virsh pool-autostart</a> <a href="#virsh-pool-autostart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable or disable autostart for a virtual machine storage pool.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### Enable autostart for the storage pool specified by name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-autostart --pool {{name|uuid}}
```
#### Disable autostart for the storage pool specified by name or UUID:
```shell
virsh pool-autostart --pool {{name|uuid}} --disable
```
{% endraw %}