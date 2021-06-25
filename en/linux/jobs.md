---
layout: default
title: "jobs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jobs">
  <a href="/en/linux/jobs.html">jobs</a> <a href="#jobs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BASH builtin for viewing information about processes spawned by the current shell.

#### View jobs spawned by the current shell:
```shell
jobs
```
#### List jobs and their process ids:
```shell
jobs -l
```
#### Display information about jobs with changed status:
```shell
jobs -n
```
#### Display process id of process group leader:
```shell
jobs -p
```
#### Display running processes:
```shell
jobs -r
```
#### Display stopped processes:
```shell
jobs -s
```
{% endraw %}