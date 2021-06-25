---
layout: default
title: "virsh pool-undefine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-undefine">
  <a href="/en/common/virsh-pool-undefine.html">virsh pool-undefine</a> <a href="#virsh-pool-undefine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete the configuration file in `/etc/libvirt/storage` for a stopped virtual machine storage pool.
> See also: `virsh`, `virsh-pool-destroy`.
> More information: <https://manned.org/virsh>.

#### Delete the configuration for the storage pool specified name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-undefine --pool {{name|uuid}}
```
{% endraw %}