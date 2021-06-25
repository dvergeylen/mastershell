---
layout: default
title: "mount"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mount">
  <a href="/en/windows/mount.html">mount</a> <a href="#mount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mount Network File System (NFS) network shares.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/mount>.

#### Mount a share to the "Z" drive letter:
```shell
mount \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share to the next available drive letter:
```shell
mount \\{{computer_name}}\{{share_name}} *
```
#### Mount a share with a read timeout in seconds (defaults to 0.8, can be 0.9 or 1 to 60):
```shell
mount -o timeout={{seconds}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share and retry up to 10 times if it fails:
```shell
mount -o retry={{retries}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share with forced case sensitivity:
```shell
mount -o casesensitive \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share as an anonymous user:
```shell
mount -o anon \\{{computer_name}}\{{share_name}} {{Z:}}
```
#### Mount a share using a specific mount type:
```shell
mount -o mtype={{soft|hard}} \\{{computer_name}}\{{share_name}} {{Z:}}
```
{% endraw %}