---
layout: default
title: "dive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dive">
  <a href="/it/common/dive.html">dive</a> <a href="#dive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un tool per esplorare immagini Docker, contenuti dei livelli, e ridurne la dimensione.
> Maggiori informazioni: <https://github.com/wagoodman/dive>.

#### Analizza un'immaigine Docker:
```shell
dive {{tag_immagine}}
```
#### Costruisci un'immagine ed avvia l'analisi:
```shell
dive build -t {{tag}}
```
{% endraw %}