---
layout: default
title: "velero"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="velero">
  <a href="/en/common/velero.html">velero</a> <a href="#velero"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Backup and migrate Kubernetes applications and their persistent volumes.
> More information: <https://github.com/heptio/velero>.

#### Create a backup containing all resources:
```shell
velero backup create {{backup_name}}
```
#### List all backups:
```shell
velero backup get
```
#### Delete a backup:
```shell
velero backup delete {{backup_name}}
```
#### Create a weekly backup, each living for 90 days (2160 hours):
```shell
velero schedule create {{schedule_name}} --schedules="{{@every 7d}}" --ttl {{2160h0m0s}}
```
#### Create a restore from the latest successful backup triggered by specific schedule:
```shell
velero restore create --from-schedule {{schedule_name}}
```
{% endraw %}