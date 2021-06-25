---
layout: default
title: "service"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="service">
  <a href="/en/linux/service.html">service</a> <a href="#service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage services by running init scripts.
> The full script path should be omitted (`/etc/init.d/` is assumed).

#### List the name and status of all services:
```shell
service --status-all
```
#### Start/Stop/Restart/Reload service (start/stop should always be available):
```shell
service {{service_name}} {{start|stop|restart|reload}}
```
#### Do a full restart (runs script twice with start and stop):
```shell
service {{service_name}} --full-restart
```
#### Show the current status of a service:
```shell
service {{service_name}} status
```
{% endraw %}