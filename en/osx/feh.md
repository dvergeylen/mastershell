---
layout: default
title: "feh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="feh">
  <a href="/en/osx/feh.html">feh</a> <a href="#feh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lightweight image viewing utility.

#### View images locally or using a URL:
```shell
feh {{path/to/images}}
```
#### View images recursively:
```shell
feh --recursive {{path/to/images}}
```
#### View images without window borders:
```shell
feh --borderless {{path/to/images}}
```
#### Exit after the last image:
```shell
feh --cycle-once {{path/to/images}}
```
#### Set the slideshow cycle delay:
```shell
feh --slideshow-delay {{seconds}} {{path/to/images}}
```
#### Set your wallpaper (centered, filled, maximized, scaled or tiled):
```shell
feh --bg-{{center|fill|max|scale|tile}} {{path/to/image}}
```
{% endraw %}