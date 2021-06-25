---
layout: default
title: "sstat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sstat">
  <a href="/en/linux/sstat.html">sstat</a> <a href="#sstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about running jobs.
> More information: <https://slurm.schedmd.com/sstat.html>.

#### Display status information of a comma-separated list of jobs:
```shell
sstat --jobs={{job_id}}
```
#### Display job ID, average CPU and average virtual memory size of a comma-separated list of jobs, with pipes as column delimiters:
```shell
sstat --parsable --jobs={{job_id}} --format={{JobID}},{{AveCPU}},{{AveVMSize}}
```
#### Display list of fields available:
```shell
sstat --helpformat
```
{% endraw %}