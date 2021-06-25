---
layout: default
title: "sinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sinfo">
  <a href="/en/linux/sinfo.html">sinfo</a> <a href="#sinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about Slurm nodes and partitions.
> See also `squeue` and `sbatch`, which are also part of the Slurm workload manager.
> More information: <https://slurm.schedmd.com/sinfo.html>.

#### Show a quick summary overview of the cluster:
```shell
sinfo --summarize
```
#### View the detailed status of all partitions across the entire cluster:
```shell
sinfo
```
#### View the detailed status of a specific partition:
```shell
sinfo --partition {{partition_name}}
```
#### View information about idle nodes:
```shell
sinfo --states {{idle}}
```
#### Summarise dead nodes:
```shell
sinfo --dead
```
#### List dead nodes and the reasons why:
```shell
sinfo --list-reasons
```
{% endraw %}