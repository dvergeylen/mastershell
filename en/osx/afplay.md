---
layout: default
title: "afplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afplay">
  <a href="/en/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line audio player.

#### Play a sound file (waits until playback ends):
```shell
afplay {{path/to/file}}
```
#### Play a sound file at 2x speed (playback rate):
```shell
afplay --rate {{2}} {{path/to/file}}
```
#### Play a sound file at half speed:
```shell
afplay --rate {{0.5}} {{path/to/file}}
```
#### Play the first N seconds of a sound file:
```shell
afplay --time {{seconds}} {{path/to/file}}
```
{% endraw %}