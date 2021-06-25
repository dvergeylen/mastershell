---
layout: default
title: "wal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wal">
  <a href="/en/common/wal.html">wal</a> <a href="#wal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to create color schemes based on the dominant colors of a wallpaper.
> More information: <https://github.com/dylanaraps/pywal>.

#### Preview color scheme:
```shell
wal --preview {{image.png}}
```
#### Create color scheme:
```shell
wal -i {{image.png}}
```
#### Create a light color scheme:
```shell
wal -il {{image.png}}
```
#### Skip setting the desktop wallpaper:
```shell
wal -in {{image.png}}
```
#### Skip setting the terminal colors:
```shell
wal -is {{image.png}}
```
#### Restore the previously generated color scheme and wallpaper:
```shell
wal -R
```
{% endraw %}