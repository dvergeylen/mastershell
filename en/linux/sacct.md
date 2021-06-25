---
layout: default
title: "sacct"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sacct">
  <a href="/en/linux/sacct.html">sacct</a> <a href="#sacct"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display accounting data from the Slurm service.
> More information: <https://slurm.schedmd.com/sacct.html>.

#### Display job id, job name, partition, account, number of allocated cpus, job state, and job exit codes for recent jobs:
```shell
sacct
```
#### Display job id, job state, job exit code for recent jobs:
```shell
sacct --brief
```
#### Display the allocations of a job:
```shell
sacct --jobs {{job_id}} --allocations
```
#### Display elapsed time, job name, number of requested CPUs, and memory requested of a job:
```shell
sacct --jobs {{job_id}} --format={{elapsed}},{{jobname}},{{reqcpus}},{{reqmem}}
```
{% endraw %}