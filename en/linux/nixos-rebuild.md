---
layout: default
title: "nixos-rebuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nixos-rebuild">
  <a href="/en/linux/nixos-rebuild.html">nixos-rebuild</a> <a href="#nixos-rebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reconfigure a NixOS machine.
> More information: <https://nixos.org/nixos/manual/#sec-changing-config>.

#### Build and switch to the new configuration, making it the boot default:
```shell
sudo nixos-rebuild switch
```
#### Build and switch to the new configuration, making it the boot default and naming the boot entry:
```shell
sudo nixos-rebuild switch -p {{name}}
```
#### Build and switch to the new configuration, making it the boot default and installing updates:
```shell
sudo nixos-rebuild switch --upgrade
```
#### Rollback changes to the configuration, switching to the previous generation:
```shell
sudo nixos-rebuild switch --rollback
```
#### Build the new configuration and make it the boot default without switching to it:
```shell
sudo nixos-rebuild boot
```
#### Build and activate the new configuration, but don't make a boot entry (for testing purposes):
```shell
sudo nixos-rebuild test
```
#### Build the configuration and open it in a virtual machine:
```shell
sudo nixos-rebuild build-vm
```
{% endraw %}