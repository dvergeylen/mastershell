---
layout: default
title: "virsh-domblklist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-domblklist">
  <a href="/en/common/virsh-domblklist.html">virsh-domblklist</a> <a href="#virsh-domblklist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about block devices associated with a virtual machine.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### List the target name and source path of the block devices:
```shell
virsh domblklist --domain {{vm_name}}
```
#### List the disk type and device value as well as the target name and source path:
```shell
virsh domblklist --domain {{vm_name}} --details
```
{% endraw %}