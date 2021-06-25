---
layout: default
title: "srun"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="srun">
  <a href="/en/linux/srun.html">srun</a> <a href="#srun"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an interactive slurm job or connect to an existing job.
> More information: <https://slurm.schedmd.com/srun.html>.

#### Submit a basic interactive job:
```shell
srun --pty /bin/bash
```
#### Submit an interactive job with different attributes:
```shell
srun --ntasks-per-node={{num_cores}} --mem-per-cpu={{memory_MB}} --pty /bin/bash
```
#### Connect to a worker node with a job running:
```shell
srun --jobid={{job_id}} --pty /bin/bash
```
{% endraw %}