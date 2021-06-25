---
layout: default
title: "pueue parallel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-parallel">
  <a href="/en/common/pueue-parallel.html">pueue parallel</a> <a href="#pueue-parallel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the amount of allowed parallel tasks.
> More information: <https://github.com/Nukesor/pueue>.

#### Set the maximum number of tasks allowed to run in parallel, in the default group:
```shell
pueue parallel {{max_number_of_parallel_tasks}}
```
#### Set the maximum number of tasks allowed to run in parallel, in a specific group:
```shell
pueue parallel --group {{group_name}} {{maximum_number_of_parallel_tasks}}
```
{% endraw %}