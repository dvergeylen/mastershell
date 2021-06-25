---
layout: default
title: "debootstrap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debootstrap">
  <a href="/en/linux/debootstrap.html">debootstrap</a> <a href="#debootstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a basic Debian system.
> More information: <https://wiki.debian.org/Debootstrap>.

#### Create a Debian stable release system inside the `debian-root` directory:
```shell
sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian
```
#### Create an Ubuntu 20.04 system inside the `focal-root` directory with a local mirror:
```shell
sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}
```
#### Switch to a bootstrapped system:
```shell
sudo chroot {{path/to/root}}
```
#### List available releases:
```shell
ls /usr/share/debootstrap/scripts/
```
{% endraw %}