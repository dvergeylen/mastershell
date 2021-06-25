---
layout: default
title: "virsh-connect"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-connect">
  <a href="/en/common/virsh-connect.html">virsh-connect</a> <a href="#virsh-connect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Connect to a virtual machine hypervisor.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### Connect to the default hypervisor:
```shell
virsh connect
```
#### Connect as root to the local QEMU/KVM hypervisor:
```shell
virsh connect qemu:///system
```
#### Launch a new instance of the hypervisor and connect to it as the local user:
```shell
virsh connect qemu:///session
```
#### Connect as root to a remote hypervisor using ssh:
```shell
virsh connect qemu+ssh://{{user_name@host_name}}/system
```
{% endraw %}