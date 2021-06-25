---
layout: default
title: "rc-update"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rc-update">
  <a href="/en/linux/rc-update.html">rc-update</a> <a href="#rc-update"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add and remove OpenRC services to and from runlevels.
> See also `openrc`.

#### List all services and the runlevels they are added to:
```shell
rc-update show
```
#### Add a service to a runlevel:
```shell
sudo rc-update add {{service_name}} {{runlevel}}
```
#### Delete a service from a runlevel:
```shell
sudo rc-update delete {{service_name}} {{runlevel}}
```
#### Delete a service from all runlevels:
```shell
sudo rc-update --all delete {{service_name}}
```
{% endraw %}