---
layout: default
title: "pueue group"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-group">
  <a href="/en/common/pueue-group.html">pueue group</a> <a href="#pueue-group"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display, add or remove groups.
> More information: <https://github.com/Nukesor/pueue>.

#### Show all groups with their statuses and number of parallel jobs:
```shell
pueue group
```
#### Add a custom group:
```shell
pueue group --add "{{group_name}}"
```
#### Remove a group and move its tasks to the default group:
```shell
pueue group --remove "{{group_name}}"
```
{% endraw %}