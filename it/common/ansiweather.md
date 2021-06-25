---
layout: default
title: "ansiweather"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansiweather">
  <a href="/it/common/ansiweather.html">ansiweather</a> <a href="#ansiweather"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uno script per mostrare le attuali condizioni meteo nel tuo terminale.
> Maggiori informazioni: <https://github.com/fcambus/ansiweather>.

#### Mostra una previsione usando unità SI per i prossimi cinque giorni in Rzeszow (Polonia):
```shell
ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}
```
#### Mostra una previsione con simboli e informazioni sulla luce solare per la tua posizione attuale:
```shell
ansiweather -s {{true}} -d {{true}}
```
#### Mostra una previsione con informazioni su vento ed umidità per la tua posizione attuale:
```shell
ansiweather -w {{true}} -h {{true}}
```
{% endraw %}