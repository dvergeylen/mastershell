---
layout: default
title: "schroot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="schroot">
  <a href="/en/linux/schroot.html">schroot</a> <a href="#schroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run command or start an interactive shell with a different root directory. More customizable than `chroot`.
> More information: <https://wiki.debian.org/Schroot>.

#### Run a command in a specific chroot:
```shell
schroot --chroot {{chroot}} {{command}}
```
#### Run a command with options in a specific chroot:
```shell
schroot --chroot {{chroot}} {{command}} -- {{command_options}}
```
#### Run a command in all available chroots:
```shell
schroot --all {{command}}
```
#### Start an interactive shell with in a specific chroot as a specific user:
```shell
schroot --chroot {{chroot}} --user {{user}}
```
#### List available chroots:
```shell
schroot --list
```
{% endraw %}