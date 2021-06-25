---
layout: default
title: "pueue restart"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-restart">
  <a href="/en/common/pueue-restart.html">pueue restart</a> <a href="#pueue-restart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restart tasks.
> More information: <https://github.com/Nukesor/pueue>.

#### Restart a specific task:
```shell
pueue restart {{task_id}}
```
#### Restart multiple tasks at once, and start them immediately (do not enqueue):
```shell
pueue restart --start-immediately {{task_id}} {{task_id}}
```
#### Restart a specific task from a different path:
```shell
pueue restart --edit-path {{task_id}}
```
#### Edit a command before restarting:
```shell
pueue restart --edit {{task_id}}
```
#### Restart a task in-place (without enqueuing as a separate task):
```shell
pueue restart --in-place {{task_id}}
```
#### Restart all failed tasks and stash them:
```shell
pueue restart --all-failed --stashed
```
{% endraw %}