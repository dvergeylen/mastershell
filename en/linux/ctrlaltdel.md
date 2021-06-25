---
layout: default
title: "ctrlaltdel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ctrlaltdel">
  <a href="/en/linux/ctrlaltdel.html">ctrlaltdel</a> <a href="#ctrlaltdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to control what happens when CTRL+ALT+DEL is pressed.

#### Get current setting:
```shell
ctrlaltdel
```
#### Set CTRL+ALT+DEL to reboot immediately, without any preparation:
```shell
sudo ctrlaltdel hard
```
#### Set CTRL+ALT+DEL to reboot "normally", giving processes a chance to exit first (send SIGINT to PID1):
```shell
sudo ctrlaltdel soft
```
{% endraw %}