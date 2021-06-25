---
layout: default
title: "pacstrap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacstrap">
  <a href="/en/linux/pacstrap.html">pacstrap</a> <a href="#pacstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux install script to install packages to the specified new root directory.
> More information: <https://man.archlinux.org/man/pacstrap.8>.

#### Install the `base` package, Linux kernel and firmware for common hardware:
```shell
pacstrap {{path/to/new/root}} {{base}} {{linux}} {{linux-firmware}}
```
#### Install the `base` package, Linux LTS kernel and `base-devel` build tools:
```shell
pacstrap {{path/to/new/root}} {{base}} {{base-devel}} {{linux-lts}}
```
#### Install packages without copy the host's mirrorlist to the target:
```shell
pacstrap -M {{path/to/new/root}} {{packages}}
```
#### Use an alternate configuration file for Pacman:
```shell
pacstrap -C {{path/to/pacman.conf}} {{path/to/new/root}} {{packages}}
```
#### Install packages using the package cache on the host instead of on the target:
```shell
pacstrap -c {{path/to/new/root}} {{packages}}
```
#### Install packages without copy the host's pacman keyring to the target:
```shell
pacstrap -G {{path/to/new/root}} {{packages}}
```
#### Install packages in interactive mode (prompts for confirmation):
```shell
pacstrap -i {{path/to/new/root}} {{packages}}
```
#### Install packages using package files:
```shell
pacstrap -U {{path/to/new/root}} {{path/to/package1}} {{path/to/package2}}
```
{% endraw %}