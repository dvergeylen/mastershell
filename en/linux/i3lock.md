---
layout: default
title: "i3lock"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="i3lock">
  <a href="/en/linux/i3lock.html">i3lock</a> <a href="#i3lock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple screen locker built for the i3 window manager.
> More information: <https://i3wm.org/i3lock>.

#### Lock screen with a simple color background (rrggbb format):
```shell
i3lock -c {{0000ff}}
```
#### Lock screen to a PNG background:
```shell
i3lock -i {{path/to/picture.png}}
```
#### Disable the unlock indicator (removes feedback on keypress):
```shell
i3lock -u
```
#### Display mouse pointer instead of hiding it ('default' for default pointer, 'win' for a MS Windows pointer):
```shell
i3lock -p {{default|win}}
```
#### Lock screen to a PNG background displayed in multiple monitors, with enabled mouse pointer:
```shell
i3lock -i {{path/to/picture.png}} -p {{default|win}} -t
```
{% endraw %}