---
layout: default
title: "virt-sysprep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virt-sysprep">
  <a href="/en/common/virt-sysprep.html">virt-sysprep</a> <a href="#virt-sysprep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reset, unconfigure, or customize a virtual machine image.
> More information: <https://manned.org/virt-sysprep>.

#### List all supported operations (enabled operations are indicated with asterisks):
```shell
virt-sysprep --list-operations
```
#### Run all enabled operations but don't actually apply the changes:
```shell
virt-sysprep --domain {{vm_name}} --dry-run
```
#### Run only the specified operations:
```shell
virt-sysprep --domain {{vm_name}} --operations {{operation1,operation2,...}}
```
#### Generate a new `/etc/machine-id` file and enable customizations to be able to change the host name to avoid network conflicts:
```shell
virt-sysprep --domain {{vm_name}} --enable {{customizations}} --hostname {{host_name}} --operation {{machine-id}}
```
{% endraw %}