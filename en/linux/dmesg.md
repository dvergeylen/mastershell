---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/en/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write the kernel messages to standard output.

#### Show kernel messages:
```shell
dmesg
```
#### Show kernel error messages:
```shell
dmesg --level err
```
#### Show kernel messages and keep reading new ones, similar to `tail -f` (available in kernels 3.5.0 and newer):
```shell
dmesg -w
```
#### Show how much physical memory is available on this system:
```shell
dmesg | grep -i memory
```
#### Show kernel messages 1 page at a time:
```shell
dmesg | less
```
#### Show kernel messages with a timestamp (available in kernels 3.5.0 and newer):
```shell
dmesg -T
```
#### Show kernel messages in human-readable form (available in kernels 3.5.0 and newer):
```shell
dmesg -H
```
#### Colorize output (available in kernels 3.5.0 and newer):
```shell
dmesg -L
```
{% endraw %}