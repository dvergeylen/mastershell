---
layout: default
title: "pueue log"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-log">
  <a href="/en/common/pueue-log.html">pueue log</a> <a href="#pueue-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the log output of 1 or more tasks.
> See also: `pueue status`.
> More information: <https://github.com/Nukesor/pueue>.

#### Show the last few lines of output from all tasks:
```shell
pueue log
```
#### Show the full output of a task:
```shell
pueue log {{task_id}}
```
#### Show the last few lines of output from several tasks:
```shell
pueue log {{task_id}} {{task_id}}
```
#### Print a specific number of lines from the tail of output:
```shell
pueue log --lines {{number_of_lines}} {{task_id}}
```
{% endraw %}