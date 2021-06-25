---
layout: default
title: "virsh-help"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="virsh-help">
  <a href="/en/common/virsh-help.html">virsh-help</a> <a href="#virsh-help"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about `virsh` commands or command groups.
> See also: `virsh`.
> More information: <https://manned.org/virsh>.

#### List the `virsh` commands grouped into related categories:
```shell
virsh help
```
#### List the command categories:
```shell
virsh help | grep "keyword"
```
#### List the commands in a category:
```shell
virsh help {{category_keyword}}
```
#### Show help for a command:
```shell
virsh help {{command}}
```
{% endraw %}