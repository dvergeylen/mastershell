---
layout: default
title: "vlc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vlc">
  <a href="/it/common/vlc.html">vlc</a> <a href="#vlc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lettore multimediale multi-piattaforma.
> Maggiori informazioni: <https://www.videolan.org/vlc/>.

#### Riproduce un file:
```shell
vlc {{percorso/al/file}}
```
#### Riproduce a schermo intero:
```shell
vlc --fullscreen {{percorso/al/file}}
```
#### Riproduce con audio disattivato:
```shell
vlc --no-audio {{percorso/al/file}}
```
#### Riproduce in ciclo continuo:
```shell
vlc --loop {{percorso/al/file}}
```
#### Riproduce il video in un certo URL:
```shell
vlc {{https://www.youtube.com/watch?v=oHg5SJYRHA0}}
```
{% endraw %}