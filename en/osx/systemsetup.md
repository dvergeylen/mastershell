---
layout: default
title: "systemsetup"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="systemsetup">
  <a href="/en/osx/systemsetup.html">systemsetup</a> <a href="#systemsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure System Preferences machine settings.

#### Enable remote login (SSH):
```shell
systemsetup -setremotelogin on
```
#### Specify TimeZone, NTP Server and enable network time:
```shell
systemsetup -settimezone {{US/Pacific}} -setnetworktimeserver {{us.pool.ntp.org}} -setusingnetworktime on
```
#### Make the machine never sleep and automatically restart on power failure or kernel panic:
```shell
systemsetup -setsleep off -setrestartpowerfailure on -setrestartfreeze on
```
#### List valid startup disks:
```shell
systemsetup -liststartupdisks
```
#### Specify a new startup disk:
```shell
systemsetup -setstartupdisk {{path}}
```
{% endraw %}