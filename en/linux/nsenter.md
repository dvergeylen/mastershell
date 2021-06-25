---
layout: default
title: "nsenter"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nsenter">
  <a href="/en/linux/nsenter.html">nsenter</a> <a href="#nsenter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a new command in a running process' namespace.
> Particularly useful for docker images or chroot jails.
> More information: <https://github.com/jpetazzo/nsenter/>.

#### Run command in existing processes network namespace:
```shell
nsenter -t {{pid}} -n {{command}} {{command_arguments}}
```
#### Run a new command in an existing processes ps-table namespace:
```shell
nsenter -t {{pid}} -p {{command}} {{command_arguments}}
```
#### Run command in existing processes IPC namespace:
```shell
nsenter -t {{pid}} -i {{command}} {{command_arguments}}
```
{% endraw %}