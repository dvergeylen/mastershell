---
layout: default
title: "virsh pool-list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-pool-list">
  <a href="/en/common/virsh-pool-list.html">virsh pool-list</a> <a href="#virsh-pool-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about virtual machine storage pools.
> See also: `virsh`, `virsh-pool-autostart`, `virsh-pool-define-as`.
> More information: <https://manned.org/virsh>.

#### List the name, state, and whether autostart is enabled or disabled for active storage pools:
```shell
virsh pool-list
```
#### List information for active and inactive or just inactive storage pools:
```shell
virsh pool-list --{{all|inactive}}
```
#### List extended information about persistence, capacity, allocation, and available space for active storage pools:
```shell
virsh pool-list --details
```
#### List information for active storage pools with either autostart enabled or disabled:
```shell
virsh pool-list --{{autostart|no-autostart}}
```
#### List information for active storage pools that are either persistent or transient:
```shell
virsh pool-list --{{persistent|transient}}
```
#### List the name and UUID of active storage pools:
```shell
virsh pool-list --name --uuid
```
{% endraw %}