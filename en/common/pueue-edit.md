---
layout: default
title: "pueue edit"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-edit">
  <a href="/en/common/pueue-edit.html">pueue edit</a> <a href="#pueue-edit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit the command or path of a stashed or queued task.
> More information: <https://github.com/Nukesor/pueue>.

#### Edit a task, see `pueue status` to get the task ID:
```shell
pueue edit {{task_id}}
```
#### Edit the path from which a task is executed:
```shell
pueue edit {{task_id}} --path
```
#### Edit a command with the specified editor:
```shell
EDITOR={{nano}} pueue edit {{task_id}}
```
{% endraw %}