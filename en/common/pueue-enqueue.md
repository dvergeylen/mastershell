---
layout: default
title: "pueue enqueue"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-enqueue">
  <a href="/en/common/pueue-enqueue.html">pueue enqueue</a> <a href="#pueue-enqueue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enqueue stashed tasks.
> See also: `pueue stash`.
> More information: <https://github.com/Nukesor/pueue>.

#### Enqueue multiple stashed tasks at once:
```shell
pueue enqueue {{task_id}} {{task_id}}
```
#### Enqueue a stashed task after 60 seconds:
```shell
pueue enqueue --delay {{60}} {{task_id}}
```
#### Enqueue a stashed task next Wednesday:
```shell
pueue enqueue --delay {{wednesday}} {{task_id}}
```
#### Enqueue a stashed task after four months:
```shell
pueue enqueue --delay "4 months" {{task_id}}
```
#### Enqueue a stashed task on 2021-02-19:
```shell
pueue enqueue --delay {{2021-02-19}} {{task_id}}
```
#### List all available date/time formats:
```shell
pueue enqueue --help
```
{% endraw %}