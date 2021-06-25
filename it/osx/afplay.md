---
layout: default
title: "afplay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afplay">
  <a href="/it/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Riproduttore audio a riga di comando.

#### Riproduci un file audio (fino a quando non finisce la riproduzione):
```shell
afplay {{percorso/del/file}}
```
#### Riproduci un file audio al doppio della velocità:
```shell
afplay --rate 2 {{percorso/del/file}}
```
#### Riproduci un file audio alla metà della velocità:
```shell
afplay --rate 0.5 {{percorso/del/file}}
```
#### Riproduci i primi N secondi di un file audio:
```shell
afplay --time {{N}} {{percorso/del/file}}
```
{% endraw %}