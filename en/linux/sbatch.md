---
layout: default
title: "sbatch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sbatch">
  <a href="/en/linux/sbatch.html">sbatch</a> <a href="#sbatch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Submit a batch job to the SLURM scheduler.

#### Submit a batch job:
```shell
sbatch {{path/to/job.sh}}
```
#### Submit a batch job with a custom name:
```shell
sbatch --job-name={{myjob}} {{path/to/job.sh}}
```
#### Submit a batch job with a time limit of 30 minutes:
```shell
sbatch --time={{00:30:00}} {{path/to/job.sh}}
```
#### Submit a job and request multiple nodes:
```shell
sbatch --nodes={{3}} {{path/to/job.sh}}
```
{% endraw %}