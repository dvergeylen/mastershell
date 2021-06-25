---
layout: default
title: "lxc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lxc">
  <a href="/en/linux/lxc.html">lxc</a> <a href="#lxc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Linux containers using the lxd REST API.
> Any container names or patterns can be prefixed with the name of a remote server.

#### List local containers matching a string. Omit the string to list all local containers:
```shell
lxc list {{match_string}}
```
#### List images matching a string. Omit the string to list all images:
```shell
lxc image list [{{remote}}:]{{match_string}}
```
#### Create a new container from an image:
```shell
lxc init [{{remote}}:]{{image}} {{container}}
```
#### Start a container:
```shell
lxc start [{{remote}}:]{{container}}
```
#### Stop a container:
```shell
lxc stop [{{remote}}:]{{container}}
```
#### Show detailed info about a container:
```shell
lxc info [{{remote}}:]{{container}}
```
#### Take a snapshot of a container:
```shell
lxc snapshot [{{remote}}:]{{container}} {{snapshot}}
```
{% endraw %}