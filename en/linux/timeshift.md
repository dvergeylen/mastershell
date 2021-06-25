---
layout: default
title: "timeshift"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="timeshift">
  <a href="/en/linux/timeshift.html">timeshift</a> <a href="#timeshift"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System restore utility.
> More information: <https://github.com/teejee2008/timeshift>.

#### List snapshots:
```shell
sudo timeshift --list
```
#### Create a new snapshot (if scheduled):
```shell
sudo timeshift --check
```
#### Create a new snapshot (even if not scheduled):
```shell
sudo timeshift --create
```
#### Restore a snapshot (selecting which snapshot to restore interactively):
```shell
sudo timeshift --restore
```
#### Restore a specific snapshot:
```shell
sudo timeshift --restore --snapshot '{{snapshot}}'
```
#### Delete a specific snapshot:
```shell
sudo timeshift --delete --snapshot '{{snapshot}}'
```
{% endraw %}