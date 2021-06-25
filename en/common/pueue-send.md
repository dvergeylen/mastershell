---
layout: default
title: "pueue send"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-send">
  <a href="/en/common/pueue-send.html">pueue send</a> <a href="#pueue-send"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send input to a task.
> More information: <https://github.com/Nukesor/pueue>.

#### Send input to a running command:
```shell
pueue send {{task_id}} "{{input}}"
```
#### Send confirmation to a task expecting y/N (e.g. apt, cp):
```shell
pueue send {{task_id}} {{y}}
```
{% endraw %}