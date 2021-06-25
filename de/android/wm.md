---
layout: default
title: "wm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wm">
  <a href="/de/android/wm.html">wm</a> <a href="#wm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über den Bildschirm eines Android-Geräts.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.

#### Gib die physische Größe des Bildschirms eines Geräts aus:
```shell
wm {{size}}
```
#### Gib die physische Pixeldichte des Bildschirms eines Geräts aus:
```shell
wm {{density}}
```
{% endraw %}