---
layout: default
title: "squeue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="squeue">
  <a href="/en/linux/squeue.html">squeue</a> <a href="#squeue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View the jobs queued in the SLURM scheduler.

#### View the queue:
```shell
squeue
```
#### View jobs queued by a specific user:
```shell
squeue -u {{username}}
```
#### View the queue and refresh every 5 seconds:
```shell
squeue -i {{5}}
```
#### View the queue with expected start times:
```shell
squeue --start
```
{% endraw %}