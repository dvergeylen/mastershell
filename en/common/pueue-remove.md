---
layout: default
title: "pueue remove"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-remove">
  <a href="/en/common/pueue-remove.html">pueue remove</a> <a href="#pueue-remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove tasks from the list. Running or paused tasks need to be killed first.
> More information: <https://github.com/Nukesor/pueue>.

#### Remove a killed or finished task:
```shell
pueue remove {{task_id}}
```
#### Remove multiple tasks at once:
```shell
pueue remove {{task_id}} {{task_id}}
```
{% endraw %}