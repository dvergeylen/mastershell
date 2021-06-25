---
layout: default
title: "VBoxManage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vboxmanage">
  <a href="/en/common/vboxmanage.html">VBoxManage</a> <a href="#vboxmanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface to VirtualBox.
> Includes all the functionality of the GUI and more.
> More information: <https://www.virtualbox.org/manual/ch08.html#vboxmanage-intro>.

#### List all VirtualBox virtual machines:
```shell
VBoxManage list vms
```
#### Show information about a particular virtual machine:
```shell
VBoxManage showvminfo {{name|uuid}}
```
#### Start a virtual machine:
```shell
VBoxManage startvm {{name|uuid}}
```
#### Start a virtual machine in headless mode:
```shell
VBoxManage startvm {{name|uuid}} -type headless
```
#### Shutdown the virtual machine and save its current state:
```shell
VBoxManage controlvm {{name|uuid}} savestate
```
#### Shutdown down the virtual machine without saving its state:
```shell
VBoxManage controlvm {{name|uuid}} poweroff
```
#### Update VBox extension packs:
```shell
VBoxManage extpack install --replace {{VboxExtensionPackFileName}}
```
{% endraw %}