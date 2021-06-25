---
layout: default
title: "pueue kill"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-kill">
  <a href="/en/common/pueue-kill.html">pueue kill</a> <a href="#pueue-kill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kill running tasks or whole groups.
> More information: <https://github.com/Nukesor/pueue>.

#### Kill all tasks in the default group:
```shell
pueue kill
```
#### Kill a specific task:
```shell
pueue kill {{task_id}}
```
#### Kill a task and terminate all its child processes:
```shell
pueue kill --children {{task_id}}
```
#### Kill all tasks in a group and pause the group:
```shell
pueue kill --group {{group_name}}
```
#### Kill all tasks across all groups and pause all groups:
```shell
pueue kill --all
```
{% endraw %}