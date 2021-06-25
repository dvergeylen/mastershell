---
layout: default
title: "svcadm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svcadm">
  <a href="/en/sunos/svcadm.html">svcadm</a> <a href="#svcadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate service instances.
> More information: <https://www.unix.com/man-page/linux/1m/svcadm>.

#### Enable a service in the service database:
```shell
svcadm enable {{service_name}}
```
#### Disable service:
```shell
svcadm disable {{service_name}}
```
#### Restart a running service:
```shell
svcadm restart {{service_name}}
```
#### Command service to re-read configuration files:
```shell
svcadm refresh {{service_name}}
```
#### Clear a service from maintenance state and command it to start:
```shell
svcadm clear {{service_name}}
```
{% endraw %}