---
layout: default
title: "minetest"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minetest">
  <a href="/en/common/minetest.html">minetest</a> <a href="#minetest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplayer infinite-world block sandbox.
> See also `minetestserver`, the server-only binary.
> More information: <https://wiki.minetest.net/Minetest>.

#### Start minetest in client mode:
```shell
minetest
```
#### Start minetest in server mode by hosting a specific world:
```shell
minetest --server --world {{name}}
```
#### Write logs to a specific file:
```shell
minetest --logfile {{path/to/file}}
```
#### Only write errors to the console:
```shell
minetest --quiet
```
{% endraw %}