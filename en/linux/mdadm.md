---
layout: default
title: "mdadm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mdadm">
  <a href="/en/linux/mdadm.html">mdadm</a> <a href="#mdadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RAID management utility.
> More information: <https://manned.org/mdadm>.

#### Create array:
```shell
mdadm --create {{/dev/md/MyRAID}} --level {{raid_level}} --raid-devices {{number_of_disks}} {{/dev/sdXN}}
```
#### Stop array:
```shell
mdadm --stop {{/dev/md0}}
```
#### Mark disk as failed:
```shell
mdadm --fail {{/dev/md0}} {{/dev/sdXN}}
```
#### Remove disk:
```shell
mdadm --remove {{/dev/md0}} {{/dev/sdXN}}
```
#### Add disk to array:
```shell
mdadm --assemble {{/dev/md0}} {{/dev/sdXN}}
```
#### Show RAID info:
```shell
mdadm --detail {{/dev/md0}}
```
{% endraw %}