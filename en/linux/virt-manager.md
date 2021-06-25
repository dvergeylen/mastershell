---
layout: default
title: "virt-manager"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virt-manager">
  <a href="/en/linux/virt-manager.html">virt-manager</a> <a href="#virt-manager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI launcher for virt-manager, a desktop user interface for managing KVM and Xen virtual machines and LXC containers.
> More information: <https://manpages.ubuntu.com/manpages/man1/virt-manager.1.html>.

#### Launch virt-manager:
```shell
virt-manager
```
#### Connect to a hypervisor:
```shell
virt-manager --connect {{hypervisor_uri}}
```
#### Don't fork virt-manager process into background on startup:
```shell
virt-manager --no-fork
```
#### Print debug output:
```shell
virt-manager --debug
```
#### Open the "New VM" wizard:
```shell
virt-manager --show-domain-creator
```
#### Show domain details window:
```shell
virt-manager --show-domain-editor {{name|id|uuid}}
```
#### Show domain performance window:
```shell
virt-manager --show-domain-performance {{name|id|uuid}}
```
#### Show connection details window:
```shell
virt-manager --show-host-summary
```
{% endraw %}