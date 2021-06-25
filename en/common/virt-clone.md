---
layout: default
title: "virt-clone"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virt-clone">
  <a href="/en/common/virt-clone.html">virt-clone</a> <a href="#virt-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clone a libvirt virtual machine.
> More information: <https://manned.org/virt-clone>.

#### Clone a virtual machine and automatically generate a new name, storage path, and MAC address:
```shell
virt-clone --original {{vm_name}} --auto-clone
```
#### Clone a virtual machine and specify the new name, storage path, and MAC address:
```shell
virt-clone --original {{vm_name}} --name {{new_vm_name}} --file {{path/to/new_storage}} --mac {{ff:ff:ff:ff:ff:ff|RANDOM}}
```
{% endraw %}