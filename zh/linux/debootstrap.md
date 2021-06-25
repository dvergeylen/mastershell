---
layout: default
title: "debootstrap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debootstrap">
  <a href="/zh/linux/debootstrap.html">debootstrap</a> <a href="#debootstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建一个基本的 `Debian` 系统。
> 更多信息：<https://wiki.debian.org/Debootstrap>.

#### 在 `debian-root` 目录中创建一个 `Debian` 稳定分支系统：
```shell
sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian
```
#### 使用本地镜像在 `focal-root` 目录中创建一个 `Ubuntu 20.04` 系统：
```shell
sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}
```
#### 切换到可引导系统：
```shell
sudo chroot {{path/to/root}}
```
#### 列出可用的版本：
```shell
ls /usr/share/debootstrap/scripts/
```
{% endraw %}