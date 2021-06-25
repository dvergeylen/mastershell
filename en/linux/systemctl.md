---
layout: default
title: "systemctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systemctl">
  <a href="/en/linux/systemctl.html">systemctl</a> <a href="#systemctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control the systemd system and service manager.
> More information: <https://www.freedesktop.org/software/systemd/man/systemctl.html>.

#### List failed units:
```shell
systemctl --failed
```
#### Start/Stop/Restart/Reload a service:
```shell
systemctl {{start|stop|restart|reload}} {{unit}}
```
#### Show the status of a unit:
```shell
systemctl status {{unit}}
```
#### Enable/Disable a unit to be started on bootup:
```shell
systemctl {{enable|disable}} {{unit}}
```
#### Mask/Unmask a unit to prevent enablement and manual activation:
```shell
systemctl {{mask|unmask}} {{unit}}
```
#### Reload systemd, scanning for new or changed units:
```shell
systemctl daemon-reload
```
#### Check if a unit is active:
```shell
systemctl is-active {{unit}}
```
#### Check if a unit is enabled:
```shell
systemctl is-enabled {{unit}}
```
{% endraw %}