---
layout: default
title: "pueue clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pueue-clean">
  <a href="/en/common/pueue-clean.html">pueue clean</a> <a href="#pueue-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove all finished tasks from the list and clear logs.
> More information: <https://github.com/Nukesor/pueue>.

#### Remove finished tasks and clear logs:
```shell
pueue clean
```
#### Only clean commands that finished successfully:
```shell
pueue clean --successful-only
```
{% endraw %}