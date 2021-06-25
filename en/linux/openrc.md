---
layout: default
title: "openrc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openrc">
  <a href="/en/linux/openrc.html">openrc</a> <a href="#openrc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The OpenRC service manager.
> See also `rc-status`, `rc-update`, and `rc-service`.
> More information: <https://wiki.gentoo.org/wiki/OpenRC>.

#### Change to a specific runlevel:
```shell
sudo openrc {{runlevel_name}}
```
#### Change to a specific runlevel, but don't stop any existing services:
```shell
sudo openrc --no-stop {{runlevel_name}}
```
{% endraw %}