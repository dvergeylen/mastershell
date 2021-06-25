---
layout: default
title: "qsub"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="qsub">
  <a href="/en/linux/qsub.html">qsub</a> <a href="#qsub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Submits a script to the queue management system TORQUE.

#### Submit a script with default settings (depends on TORQUE settings):
```shell
qsub {{script.sh}}
```
#### Submit a script with a specified wallclock runtime limit of 1 hour, 2 minutes and 3 seconds:
```shell
qsub -l walltime={{1}}:{{2}}:{{3}} {{script.sh}}
```
#### Submit a script that is executed on 2 nodes using 4 cores per node:
```shell
qsub -l nodes={{2}}:ppn={{4}} {{script.sh}}
```
#### Submit a script to a specific queue. Note that different queues can have different maximum and minimum runtime limits:
```shell
qsub -q {{queue_name}} {{script.sh}}
```
{% endraw %}