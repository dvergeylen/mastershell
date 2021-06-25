---
layout: default
title: "virsh-undefine"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-undefine">
  <a href="/en/common/virsh-undefine.html">virsh-undefine</a> <a href="#virsh-undefine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete a virtual machine.
> More information: <https://manned.org/virsh>.

#### Delete only the virtual machine configuration file:
```shell
virsh undefine --domain {{vm_name}}
```
#### Delete the configuration file and all associated storage volumes:
```shell
virsh undefine --domain {{vm_name}} --remove-all-storage
```
#### Delete the configuration file and the specified storage volumes using the target name or the source name (as obtained from the `virsh domblklist` command):
```shell
virsh undefine --domain {{vm_name}} --storage {{sda,path/to/source}}
```
{% endraw %}