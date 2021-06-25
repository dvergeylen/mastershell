---
layout: default
title: "renice"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="renice">
  <a href="/en/common/renice.html">renice</a> <a href="#renice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alters the scheduling priority/nicenesses of one or more running processes.
> Niceness values range from -20 (most favorable to the process) to 19 (least favorable to the process).

#### Change priority of a running process:
```shell
renice -n {{niceness_value}} -p {{pid}}
```
#### Change priority of all processes owned by a user:
```shell
renice -n {{niceness_value}} -u {{user}}
```
#### Change priority of all processes that belong to a process group:
```shell
renice -n {{niceness_value}} --pgrp {{process_group}}
```
{% endraw %}