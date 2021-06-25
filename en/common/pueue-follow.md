---
layout: default
title: "pueue follow"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-follow">
  <a href="/en/common/pueue-follow.html">pueue follow</a> <a href="#pueue-follow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Follow the output of a currently running task.
> See also: `pueue log`.
> More information: <https://github.com/Nukesor/pueue>.

#### Follow the output of a task (stdout + stderr):
```shell
pueue follow {{task_id}}
```
#### Follow the stderr of a task:
```shell
pueue follow --err {{task_id}}
```
{% endraw %}