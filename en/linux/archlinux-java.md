---
layout: default
title: "archlinux-java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="archlinux-java">
  <a href="/en/linux/archlinux-java.html">archlinux-java</a> <a href="#archlinux-java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A helper script that provides functionalities for Java environments.
> More information: <https://github.com/michaellass/archlinux-java-run>.

#### List installed Java environments:
```shell
archlinux-java status
```
#### Set the default Java environment:
```shell
archlinux-java set {{java_environment}}
```
#### Unset the default Java environment:
```shell
archlinux-java unset
```
#### Set the default Java environment automatically:
```shell
archlinux-java fix
```
{% endraw %}