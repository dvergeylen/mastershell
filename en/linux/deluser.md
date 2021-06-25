---
layout: default
title: "deluser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="deluser">
  <a href="/en/linux/deluser.html">deluser</a> <a href="#deluser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete a user from the system.
> Note: all commands must be executed as root.
> More information: <https://manpages.debian.org/latest/adduser/deluser.html>.

#### Remove a user:
```shell
deluser {{username}}
```
#### Remove a user and their home directory:
```shell
deluser --remove-home {{username}}
```
#### Remove a user and their home, but backup their files into a `.tar.gz` file in the specified directory:
```shell
deluser --backup-to {{path/to/backup_directory}} --remove-home {{username}}
```
#### Remove a user, and all files owned by them:
```shell
deluser --remove-all-files {{username}}
```
{% endraw %}