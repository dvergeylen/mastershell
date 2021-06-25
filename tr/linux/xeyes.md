---
layout: default
title: "xeyes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xeyes">
  <a href="/tr/linux/xeyes.html">xeyes</a> <a href="#xeyes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ekranda fare imlecini takip eden bir çift göz göster.

#### Xeyes'ı yerel makinenin varsayılan ekranında başlat:
```shell
xeyes
```
#### Xeyes'ı uzak bir makinenin 0. görüntü ve 0. ekran koordinatlarında başlat:
```shell
xeyes -display {{uzak_makine}}:{{0}}.{{0}}
```
{% endraw %}