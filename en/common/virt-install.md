---
layout: default
title: "virt-install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virt-install">
  <a href="/en/common/virt-install.html">virt-install</a> <a href="#virt-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create virtual machines with libvirt and begin OS installation.
> More information: <https://virt-manager.org/>.

#### Create a virtual machine with 1 GiB RAM and 12 GiB storage and start Debian installation:
```shell
virt-install --name {{vm_name}} --memory {{1024}} --disk path={{path/to/image.qcow2}},size={{12}} --cdrom {{path/to/debian.iso}}
```
{% endraw %}