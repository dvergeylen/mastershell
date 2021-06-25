---
layout: default
title: "quota"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="quota">
  <a href="/en/common/quota.html">quota</a> <a href="#quota"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display users' disk space usage and allocated limits.

#### Show disk quotas in human readable units for the current user:
```shell
quota -s
```
#### Verbose output (also display quotas on filesystems where no storage is allocated):
```shell
quota -v
```
#### Quiet output (only display quotas on filesystems where usage is over quota):
```shell
quota -q
```
#### Print quotas for the groups of which the current user is a member:
```shell
quota -g
```
#### Show disk quotas for another user:
```shell
sudo quota -u {{username}}
```
{% endraw %}