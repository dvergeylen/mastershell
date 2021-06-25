---
layout: default
title: "pmset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pmset">
  <a href="/en/osx/pmset.html">pmset</a> <a href="#pmset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure macOS power management settings, as one might do in System Preferences > Energy Saver.
> Commands that modify settings must begin with `sudo`.

#### Display the current power management settings:
```shell
pmset -g
```
#### Display the current power source and battery levels:
```shell
pmset -g batt
```
#### Put display to sleep immediately:
```shell
pmset displaysleepnow
```
#### Set display to never sleep when on charger power:
```shell
sudo pmset -c displaysleep 0
```
#### Set display to sleep after 15 minutes when on battery power:
```shell
sudo pmset -b displaysleep 15
```
#### Schedule computer to automatically wake up every weekday at 9 AM:
```shell
sudo pmset repeat wake MTWRF 09:00:00
```
#### Restore to system defaults:
```shell
sudo pmset -a displaysleep 10 disksleep 10 sleep 30 womp 1
```
{% endraw %}