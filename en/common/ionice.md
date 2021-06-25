---
layout: default
title: "ionice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ionice">
  <a href="/en/common/ionice.html">ionice</a> <a href="#ionice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set program I/O scheduling class and priority.
> Scheduling classes: 1 (realtime), 2 (best-effort), 3 (idle).
> Priority levels: 0 (the highest) - 7 (the lowest).

#### Set I/O scheduling class of a running process:
```shell
ionice -c {{scheduling_class}} -p {{pid}}
```
#### Run a command with custom I/O scheduling class and priority:
```shell
ionice -c {{scheduling_class}} -n {{priority}} {{command}}
```
#### Print the I/O scheduling class and priority of a running process:
```shell
ionice -p {{pid}}
```
{% endraw %}