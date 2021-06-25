---
layout: default
title: "pueue reset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-reset">
  <a href="/en/common/pueue-reset.html">pueue reset</a> <a href="#pueue-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kill everything and reset.
> More information: <https://github.com/Nukesor/pueue>.

#### Kill all tasks and remove everything (logs, status, groups, task IDs):
```shell
pueue reset
```
#### Kill all tasks, terminate their children, and reset everything:
```shell
pueue reset --children
```
#### Reset without asking for confirmation:
```shell
pueue reset --force
```
{% endraw %}