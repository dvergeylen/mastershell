---
layout: default
title: "edquota"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="edquota">
  <a href="/en/linux/edquota.html">edquota</a> <a href="#edquota"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit quotas for a user or group. By default it operates on all filesystems with quotas.
> Quota information is stored permanently in the `quota.user` and `quota.group` files in the root of the filesystem.

#### Edit quota of the current user:
```shell
edquota --user $(whoami)
```
#### Edit quota of a specific user:
```shell
sudo edquota --user {{username}}
```
#### Edit quota for a group:
```shell
sudo edquota --group {{group}}
```
#### Restrict operations to a given filesystem (by default edquota operates on all filesystems with quotas):
```shell
sudo edquota --file-system {{filesystem}}
```
#### Edit the default grace period:
```shell
sudo edquota -t
```
#### Duplicate a quota to other users:
```shell
sudo edquota -p {{reference_user}} {{destination_user1}} {{destination_user2}}
```
{% endraw %}