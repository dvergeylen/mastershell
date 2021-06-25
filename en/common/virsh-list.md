---
layout: default
title: "virsh-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-list">
  <a href="/en/common/virsh-list.html">virsh-list</a> <a href="#virsh-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List the ID, name, and state of virtual machines.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### List information about running virtual machines:
```shell
virsh list
```
#### List information about virtual machines regardless of state:
```shell
virsh list --all
```
#### List information about virtual machines with autostart either enabled or disabled:
```shell
virsh list --all --{{autostart|no-autostart}}
```
#### List information about virtual machines either with or without snapshots:
```shell
virsh list --all --{{with-snapshot|without-snapshot}}
```
{% endraw %}