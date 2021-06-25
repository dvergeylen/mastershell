---
layout: default
title: "update-rc.d"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="update-rc.d">
  <a href="/en/linux/update-rc.d.html">update-rc.d</a> <a href="#update-rc.d"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install and remove services which are System-V style init script links.
> Init scripts are in the `/etc/init.d/`.

#### Install a service:
```shell
update-rc.d {{mysql}} defaults
```
#### Enable a service:
```shell
update-rc.d {{mysql}} enable
```
#### Disable a service:
```shell
update-rc.d {{mysql}} disable
```
#### Forcibly remove a service:
```shell
update-rc.d -f {{mysql}} remove
```
{% endraw %}