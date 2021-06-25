---
layout: default
title: "mocp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mocp">
  <a href="/en/linux/mocp.html">mocp</a> <a href="#mocp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Music on Console (MOC) audio player.
> More information: <https://manned.org/mocp>.

#### Launch the MOC terminal UI:
```shell
mocp
```
#### Launch the MOC terminal UI in a specific directory:
```shell
mocp {{path/to/directory}}
```
#### Start the MOC server in the background, without launching the MOC terminal UI:
```shell
mocp --server
```
#### Add a specific song to the play queue while MOC is in the background:
```shell
mocp --enqueue {{path/to/audio_file}}
```
#### Add songs recursively to the play queue while MOC is in the background:
```shell
mocp --append {{path/to/directory}}
```
#### Clear the play queue while MOC is in the background:
```shell
mocp --clear
```
#### Play or stop the currently queued song while MOC is in the background:
```shell
mocp --{{play|stop}}
```
#### Stop the MOC server while it's in the background:
```shell
mocp --exit
```
{% endraw %}