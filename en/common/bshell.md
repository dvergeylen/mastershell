---
layout: default
title: "bshell"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bshell">
  <a href="/en/common/bshell.html">bshell</a> <a href="#bshell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A GUI tool for browsing for SSH/VNC servers on the local network.
> See also: `bssh` and `bvnc`.
> More information: <https://linux.extremeoverclocking.com/man/1/bssh>.

#### Browse for both SSH and VNC servers:
```shell
bshell
```
#### Browse for SSH servers only:
```shell
bshell --ssh
```
#### Browse for VNC servers only:
```shell
bshell --vnc
```
#### Browse for both SSH and VNC servers in a specified domain:
```shell
bshell --domain={{domain}}
```
{% endraw %}