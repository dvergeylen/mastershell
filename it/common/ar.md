---
layout: default
title: "ar"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ar">
  <a href="/it/common/ar.html">ar</a> <a href="#ar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, modifica ed estrai da archivi (`.a`, `.so`, `.o`).
> Maggiori informazioni: <https://manned.org/ar>.

#### Estrai tutti i membri da un archivio:
```shell
ar -x {{libfoo.a}}
```
#### Lista tutti i membri di un archivio:
```shell
ar -t {{libfoo.a}}
```
#### Sostituisci o aggiungi file ad un archvio:
```shell
ar -r {{libfoo.a}} {{foo.o}} {{bar.o}} {{baz.o}}
```
#### Inserisci o sostituisci un indice in un archivio (equivalente ad usare `ranlib`):
```shell
ar -s {{libfoo.a}}
```
#### Crea un archivio con dei file creando anche il relativo indice:
```shell
ar -rs {{libfoo.a}} {{foo.o}} {{bar.o}} {{baz.o}}
```
{% endraw %}