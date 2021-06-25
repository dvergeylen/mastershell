---
layout: default
title: "virsh pool-build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-build">
  <a href="/en/common/virsh-pool-build.html">virsh pool-build</a> <a href="#virsh-pool-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build the underlying storage system for a virtual machine storage pool as defined in it's configuration file in `/etc/libvirt/storage`.
> See also: `virsh`, `virsh-pool-define-as`, `virsh-pool-start`.
> More information: <https://manned.org/virsh>.

#### Build the storage pool specified by name or UUID (determine using `virsh pool-list`):
```shell
virsh pool-build --pool {{name|uuid}}
```
{% endraw %}