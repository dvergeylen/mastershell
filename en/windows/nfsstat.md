---
layout: default
title: "nfsstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nfsstat">
  <a href="/en/windows/nfsstat.html">nfsstat</a> <a href="#nfsstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or reset the number of calls made to the NFS server.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/nfsstat>.

#### Display the recorded number of calls made to the NFS server:
```shell
nfsstat
```
#### Reset the recorded number of calls made to the NFS server:
```shell
nfsstat -z
```
{% endraw %}