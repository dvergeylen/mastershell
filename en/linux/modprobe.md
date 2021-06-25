---
layout: default
title: "modprobe"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="modprobe">
  <a href="/en/linux/modprobe.html">modprobe</a> <a href="#modprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add or remove modules from the Linux kernel.

#### Pretend to load a module into the kernel, but don't actually do it:
```shell
sudo modprobe --dry-run {{module_name}}
```
#### Load a module into the kernel:
```shell
sudo modprobe {{module_name}}
```
#### Remove a module from the kernel:
```shell
sudo modprobe --remove {{module_name}}
```
#### Remove a module and those that depend on it from the kernel:
```shell
sudo modprobe --remove-dependencies {{module_name}}
```
#### Show a kernel module's dependencies:
```shell
sudo modprobe --show-depends {{module_name}}
```
{% endraw %}