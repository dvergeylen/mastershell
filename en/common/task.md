---
layout: default
title: "task"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="task">
  <a href="/en/common/task.html">task</a> <a href="#task"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> TODO list manager.

#### Add new task:
```shell
task add {{thing_to_do}}
```
#### List tasks:
```shell
task list
```
#### Mark task as completed:
```shell
task {{task_id}} done
```
#### Modify task:
```shell
task {{task_id}} modify {{new_thing_to_do}}
```
#### Delete task:
```shell
task {{task_id}} delete
```
{% endraw %}