---
layout: default
title: "scontrol"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scontrol">
  <a href="/en/linux/scontrol.html">scontrol</a> <a href="#scontrol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about and modify jobs.
> More information: <https://slurm.schedmd.com/scontrol.html>.

#### Show information for job:
```shell
scontrol show job {{job_id}}
```
#### Suspend a comma-separated list of running jobs:
```shell
scontrol suspend {{job_id}}
```
#### Resume a comma-separated list of suspended jobs:
```shell
scontrol resume {{job_id}}
```
#### Hold a comma-separated list of queued jobs (Use `release` command to permit the jobs to be scheduled):
```shell
scontrol hold {{job_id}}
```
#### Release a comma-separated list of suspended job:
```shell
scontrol release {{job_id}}
```
{% endraw %}