---
layout: default
title: "showmount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="showmount">
  <a href="/en/windows/showmount.html">showmount</a> <a href="#showmount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about NFS filesystems on Windows Server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/showmount>.

#### Display all exported filesystems:
```shell
showmount -e
```
#### Display all NFS clients and their mounted directories:
```shell
showmount -a
```
#### Display all NFS mounted directories:
```shell
showmount -d
```
#### Display all exported filesystems for a remote server:
```shell
showmount -e {{server_address}}
```
{% endraw %}