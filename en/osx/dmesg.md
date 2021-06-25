---
layout: default
title: "dmesg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmesg">
  <a href="/en/osx/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write the kernel messages to standard output.

#### Show kernel messages:
```shell
dmesg
```
#### Show how much physical memory is available on this system:
```shell
dmesg | grep -i memory
```
#### Show kernel messages 1 page at a time:
```shell
dmesg | less
```
{% endraw %}