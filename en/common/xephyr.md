---
layout: default
title: "Xephyr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xephyr">
  <a href="/en/common/xephyr.html">Xephyr</a> <a href="#xephyr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A nested X server that runs as an X application.

#### Create a black window with display ID ":2":
```shell
Xephyr -br -ac -noreset -screen {{800x600}} {{:2}}
```
#### Start an X application on the new screen:
```shell
DISPLAY=:2 {{command_name}}
```
{% endraw %}