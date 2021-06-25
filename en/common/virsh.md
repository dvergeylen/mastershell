---
layout: default
title: "virsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh">
  <a href="/en/common/virsh.html">virsh</a> <a href="#virsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage virsh guest domains.
> NOTE: 'guest_id' can be the id, name or UUID of the guest.
> More information: <https://libvirt.org/virshcmdref.html>.

#### Connect to a hypervisor session:
```shell
virsh connect {{qemu:///system}}
```
#### List all domains:
```shell
virsh list --all
```
#### Dump guest configuration file:
```shell
virsh dumpxml {{guest_id}} > {{path/to/guest.xml}}
```
#### Create a guest from a configuration file:
```shell
virsh create {{path/to/config_file.xml}}
```
#### Edit a guest's configuration file (editor can be changed with $EDITOR):
```shell
virsh edit {{guest_id}}
```
#### Start/reboot/shutdown/suspend/resume a guest:
```shell
virsh {{command}} {{guest_id}}
```
#### Save the current state of a guest to a file:
```shell
virsh save {{guest_id}} {{filename}}
```
#### Delete a running guest:
```shell
virsh destroy {{guest_id}} && virsh undefine {{guest_id}}
```
{% endraw %}