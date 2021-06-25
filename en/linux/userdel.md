---
layout: default
title: "userdel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="userdel">
  <a href="/en/linux/userdel.html">userdel</a> <a href="#userdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a user account or remove a user from a group.
> Note: all commands must be executed as root.
> More information: <https://manned.org/userdel>.

#### Remove a user:
```shell
userdel {{name}}
```
#### Remove a user along with their home directory and mail spool:
```shell
userdel --remove {{name}}
```
#### Remove a user from a group:
```shell
userdel {{name}} {{group}}
```
#### Remove a user in other root directory:
```shell
userdel --root {{path/to/other/root}} {{name}}
```
{% endraw %}