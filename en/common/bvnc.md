---
layout: default
title: "bvnc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bvnc">
  <a href="/en/common/bvnc.html">bvnc</a> <a href="#bvnc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A GUI tool for browsing for SSH/VNC servers on the local network.
> See also: `bssh` and `bshell`.
> More information: <https://linux.extremeoverclocking.com/man/1/bssh>.

#### Browse for VNC servers:
```shell
bvnc
```
#### Browse for SSH servers:
```shell
bvnc --ssh
```
#### Browse for both VNC and SSH servers:
```shell
bvnc --shell
```
#### Browse for VNC servers in a specified domain:
```shell
bvnc --domain={{domain}}
```
{% endraw %}