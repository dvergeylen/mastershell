---
layout: default
title: "playerctl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="playerctl">
  <a href="/en/linux/playerctl.html">playerctl</a> <a href="#playerctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to control different media players.
> More information: <https://github.com/altdesktop/playerctl>.

#### Toggle play:
```shell
playerctl play-pause
```
#### Next media:
```shell
playerctl next
```
#### Previous media:
```shell
playerctl previous
```
#### List all players:
```shell
playerctl --list-all
```
#### Send a command to a specific player:
```shell
playerctl --player={{player_name}} {{command}}
```
#### Send a command to all players:
```shell
playerctl --all-players {{command}}
```
#### Show now playing:
```shell
playerctl metadata --format "Now playing: {{artist}} - {{album}} - {{title}}"
```
{% endraw %}