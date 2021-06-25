---
layout: default
title: "chkconfig"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chkconfig">
  <a href="/en/linux/chkconfig.html">chkconfig</a> <a href="#chkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the runlevel of services on CentOS 6.

#### List services with runlevel:
```shell
chkconfig --list
```
#### Show a service's runlevel:
```shell
chkconfig --list {{ntpd}}
```
#### Enable service at boot:
```shell
chkconfig {{sshd}} on
```
#### Enable service at boot for runlevels 2, 3, 4, and 5:
```shell
chkconfig --level {{2345}} {{sshd}} on
```
#### Disable service at boot:
```shell
chkconfig {{ntpd}} off
```
#### Disable service at boot for runlevel 3:
```shell
chkconfig --level {{3}} {{ntpd}} off
```
{% endraw %}