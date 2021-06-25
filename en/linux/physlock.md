---
layout: default
title: "physlock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="physlock">
  <a href="/en/linux/physlock.html">physlock</a> <a href="#physlock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lock all consoles and virtual terminals.
> More information: <http://github.com/muennich/physlock>.

#### Lock every console (require current user or root to unlock):
```shell
physlock
```
#### Mute kernel messages on console while locked:
```shell
physlock -m
```
#### Disable SysRq mechanism while locked:
```shell
physlock -s
```
#### Display a message before the password prompt:
```shell
physlock -p "{{Locked!}}"
```
#### Fork and detach physlock (useful for suspend or hibernate scripts):
```shell
physlock -d
```
{% endraw %}