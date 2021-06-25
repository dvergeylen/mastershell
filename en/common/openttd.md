---
layout: default
title: "openttd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="openttd">
  <a href="/en/common/openttd.html">openttd</a> <a href="#openttd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open source clone of the Microprose game "Transport Tycoon Deluxe".
> More information: <https://www.openttd.org>.

#### Start a new game:
```shell
openttd -g
```
#### Load save game at start:
```shell
openttd -g {{path/to/file}}
```
#### Start with the specified window resolution:
```shell
openttd -r {{1920x1080}}
```
#### Start with a custom configuration file:
```shell
openttd -c {{path/to/file}}
```
#### Start with selected video, sound, and music drivers:
```shell
openttd -v {{video_driver}} -s {{sound_driver}} -m {{music_driver}}
```
#### Start a dedicated server, forked in the background:
```shell
openttd -f -D {{host}}:{{port}}
```
#### Join a server with a password:
```shell
openttd -n {{host}}:{{port}}#{{player_name}} -p {{password}}
```
{% endraw %}