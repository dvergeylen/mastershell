---
layout: default
title: "bssh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bssh">
  <a href="/en/common/bssh.html">bssh</a> <a href="#bssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A GUI tool for browsing for SSH/VNC servers on the local network.
> See also: `bvnc` and `bshell`.
> More information: <https://linux.extremeoverclocking.com/man/1/bssh>.

#### Browse for SSH servers:
```shell
bssh
```
#### Browse for VNC servers:
```shell
bssh --vnc
```
#### Browse for both SSH and VNC servers:
```shell
bssh --shell
```
#### Browse for SSH servers in a specified domain:
```shell
bssh --domain={{domain}}
```
{% endraw %}