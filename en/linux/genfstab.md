---
layout: default
title: "genfstab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="genfstab">
  <a href="/en/linux/genfstab.html">genfstab</a> <a href="#genfstab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux install script to generate output suitable for addition to an fstab file.
> More information: <https://man.archlinux.org/man/extra/arch-install-scripts/genfstab.8>.

#### Display an fstab compatible output based on a volume label:
```shell
genfstab -L {{path/to/mount_point}}
```
#### Display an fstab compatible output based on a volume UUID:
```shell
genfstab -U {{path/to/mount_point}}
```
#### A usual way to generate an fstab file, requires root permissions:
```shell
genfstab -U {{/mnt}} >> {{/mnt/etc/fstab}}
```
#### Append a volume into an fstab file to mount it automatically:
```shell
genfstab -U {{path/to/mount_point}} | sudo tee -a /etc/fstab
```
{% endraw %}