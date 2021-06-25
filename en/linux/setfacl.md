---
layout: default
title: "setfacl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="setfacl">
  <a href="/en/linux/setfacl.html">setfacl</a> <a href="#setfacl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set file access control lists (ACL).

#### Modify ACL of a file for user with read and write access:
```shell
setfacl -m u:{{username}}:rw {{file}}
```
#### Modify default ACL of a file for all users:
```shell
setfacl -d -m u::rw {{file}}
```
#### Remove ACL of a file for an user:
```shell
setfacl -x u:{{username}} {{file}}
```
#### Remove all ACL entries of a file:
```shell
setfacl -b {{file}}
```
{% endraw %}