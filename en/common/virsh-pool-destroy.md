---
layout: default
title: "virsh pool-destroy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-destroy">
  <a href="/en/common/virsh-pool-destroy.html">virsh pool-destroy</a> <a href="#virsh-pool-destroy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stop an active virtual machine storage pool.
> See also: `virsh`, `virsh-pool-delete`.
> More information: <https://manned.org/virsh>.

#### Stop a storage pool specified by name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-destroy --pool {{name|uuid}}
```
{% endraw %}