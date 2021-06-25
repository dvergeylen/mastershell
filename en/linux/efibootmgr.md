---
layout: default
title: "efibootmgr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="efibootmgr">
  <a href="/en/linux/efibootmgr.html">efibootmgr</a> <a href="#efibootmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate the UEFI Boot Manager.
> More information: <https://manned.org/efibootmgr>.

#### List the current settings / bootnums:
```shell
efibootmgr
```
#### List the filepaths:
```shell
efibootmgr -v
```
#### Add UEFI Shell v2 as a boot option:
```shell
sudo efibootmgr -c -d {{/dev/sda1}} -l {{\EFI\tools\Shell.efi}} -L "{{UEFI Shell}}"
```
#### Change the current boot order:
```shell
sudo efibootmgr -o {{0002,0008,0001,0005}}
```
#### Delete a boot option:
```shell
sudo efibootmgr -b {{0008}} --delete-bootnum
```
{% endraw %}