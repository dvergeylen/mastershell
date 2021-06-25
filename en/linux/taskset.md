---
layout: default
title: "taskset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="taskset">
  <a href="/en/linux/taskset.html">taskset</a> <a href="#taskset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set a process' CPU affinity or start a new process with a defined CPU affinity.

#### Get a running process' CPU affinity by PID:
```shell
taskset --pid --cpu-list {{pid}}
```
#### Set a running process' CPU affinity by PID:
```shell
taskset --pid --cpu-list {{cpu_id}} {{pid}}
```
#### Start a new process with affinity for a single CPU:
```shell
taskset --cpu-list {{cpu_id}} {{command}}
```
#### Start a new process with affinity for multiple non-sequential CPUs:
```shell
taskset --cpu-list {{cpu_id_1}} {{cpu_id_2}} {{cpu_id_3}}
```
#### Start a new process with affinity for CPUs 1 through 4:
```shell
taskset --cpu-list {{cpu_id_1}},{{cpu_id_4}}
```
{% endraw %}