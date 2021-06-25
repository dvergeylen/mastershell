---
layout: default
title: "pueue start"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-start">
  <a href="/en/common/pueue-start.html">pueue start</a> <a href="#pueue-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resume operation of specific tasks or groups of tasks.
> See also: `pueue pause`.
> More information: <https://github.com/Nukesor/pueue>.

#### Resume all tasks in the default group:
```shell
pueue start
```
#### Resume a specific task:
```shell
pueue start {{task_id}}
```
#### Resume multiple tasks at once:
```shell
pueue start {{task_id}} {{task_id}}
```
#### Resume all tasks and start their children:
```shell
pueue start --all --children
```
#### Resume all tasks in a specific group:
```shell
pueue start group {{group_name}}
```
{% endraw %}