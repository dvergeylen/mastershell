---
layout: default
title: "rc-service"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rc-service">
  <a href="/en/linux/rc-service.html">rc-service</a> <a href="#rc-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Locate and run OpenRC services with arguments.
> See also `openrc`.

#### Show a service's status:
```shell
rc-service {{service_name}} status
```
#### Start a service:
```shell
sudo rc-service {{service_name}} start
```
#### Stop a service:
```shell
sudo rc-servie {{service_name}} stop
```
#### Restart a service:
```shell
sudo rc-service {{service_name}} restart
```
#### Simulate running a service's custom command:
```shell
sudo rc-service --dry-run {{service_name}} {{command_name}}
```
#### Actually run a service's custom command:
```shell
sudo rc-service {{service_name}} {{command_name}}
```
#### Resolve the location of a service definition on disk:
```shell
sudo rc-service --resolve {{service_name}}
```
{% endraw %}