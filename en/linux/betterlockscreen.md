---
layout: default
title: "betterlockscreen"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="betterlockscreen">
  <a href="/en/linux/betterlockscreen.html">betterlockscreen</a> <a href="#betterlockscreen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple, minimal lock screen.

#### Lock the screen:
```shell
betterlockscreen --lock
```
#### Change the lock screen background:
```shell
betterlockscreen -u {{path/to/image.png}}
```
#### Lock the screen, showing some custom text:
```shell
betterlockscreen -l pixel -t "{{custom lock screen text}}"
```
#### Lock the screen, with a custom monitor off timeout in seconds:
```shell
betterlockscreen --off {{5}} -l
```
{% endraw %}