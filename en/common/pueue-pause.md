---
layout: default
title: "pueue pause"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-pause">
  <a href="/en/common/pueue-pause.html">pueue pause</a> <a href="#pueue-pause"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pause running tasks or groups.
> See also: `pueue start`.
> More information: <https://github.com/Nukesor/pueue>.

#### Pause all tasks in the default group:
```shell
pueue pause
```
#### Pause a running task:
```shell
pueue pause {{task_id}}
```
#### Pause a running task and stop all its direct children:
```shell
pueue pause --children {{task_id}}
```
#### Pause all tasks in a group and prevent it from starting new tasks:
```shell
pueue pause --group {{group_name}}
```
#### Pause all tasks and prevent all groups from starting new tasks:
```shell
pueue pause --all
```
{% endraw %}