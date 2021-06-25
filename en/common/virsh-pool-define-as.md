---
layout: default
title: "virsh pool-define-as"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-define-as">
  <a href="/en/common/virsh-pool-define-as.html">virsh pool-define-as</a> <a href="#virsh-pool-define-as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a configuration file in `/etc/libvirt/storage` for a persistent virtual machine storage pool from the provided arguments.
> See also: `virsh`, `virsh-pool-build`, `virsh-pool-start`.
> More information: <https://manned.org/virsh>.

#### Create the configuration file for a storage pool called pool_name using `/var/vms` as the underlying storage system:
```shell
virsh pool-define-as --name {{pool_name}} --type {{dir}} --target {{/var/vms}}
```
{% endraw %}