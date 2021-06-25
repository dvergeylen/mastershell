---
layout: default
title: "sacctmgr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sacctmgr">
  <a href="/en/linux/sacctmgr.html">sacctmgr</a> <a href="#sacctmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, setup, and manage Slurm accounts.
> More information: <https://slurm.schedmd.com/sacctmgr.html>.

#### Show current configuration:
```shell
sacctmgr show configuration
```
#### Add a cluster to the slurm database:
```shell
sacctmgr add cluster {{cluster_name}}
```
#### Add an account to the slurm database:
```shell
sacctmgr add account {{account_name}} cluster={{cluster_of_account}}
```
#### Show details of user/association/cluster/account:
```shell
sacctmgr show {{user/association/cluster/account}}
```
{% endraw %}