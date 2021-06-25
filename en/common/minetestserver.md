---
layout: default
title: "minetestserver"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="minetestserver">
  <a href="/en/common/minetestserver.html">minetestserver</a> <a href="#minetestserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplayer infinite-world block sandbox server.
> See also `minetest`, the graphical client.
> More information: <https://wiki.minetest.net/Setting_up_a_server>.

#### Start the server:
```shell
minetestserver
```
#### List available worlds:
```shell
minetestserver --world list
```
#### Specify the world name to load:
```shell
minetestserver --world {{world_name}}
```
#### List the available game IDs:
```shell
minetestserver --gameid list
```
#### Specify a game to use:
```shell
minetestserver --gameid {{game_id}}
```
#### Listen on a specific port:
```shell
minetestserver --port {{34567}}
```
#### Migrate to a different data backend:
```shell
minetestserver --migrate {{sqlite3|leveldb|redis}}
```
#### Start an interactive terminal after starting the server:
```shell
minetestserver --terminal
```
{% endraw %}