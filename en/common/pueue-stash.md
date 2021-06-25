---
layout: default
title: "pueue stash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-stash">
  <a href="/en/common/pueue-stash.html">pueue stash</a> <a href="#pueue-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stash tasks to prevent them starting automatically.
> See also `pueue start` and `pueue enqueue`.
> More information: <https://github.com/Nukesor/pueue>.

#### Stash an enqueued task:
```shell
pueue stash {{task_id}}
```
#### Stash multiple tasks at once:
```shell
pueue stash {{task_id}} {{task_id}}
```
#### Start a stashed task immediately:
```shell
pueue start {{task_id}}
```
#### Enqueue a task to be executed when preceding tasks finish:
```shell
pueue enqueue {{task_id}}
```
{% endraw %}