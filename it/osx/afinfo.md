---
layout: default
title: "afinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="afinfo">
  <a href="/it/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizzatore dei metadata dei file audio per macOS.
> Comando integrato di macOS.

#### Mostra le informazioni relative ad un file audio specificato:
```shell
afinfo {{percorso/del/file}}
```
#### Mostra una breve descrizione del file audio:
```shell
afinfo -b {{percorso/del/file}}
```
#### Mostra i metadati ed i contenuti dell'InfoDictionary del file audio:
```shell
afinfo -i {{percorso/del/file}}
```
#### Mostra l'output in formato xml:
```shell
afinfo -x {{percorso/del/file}}
```
#### Mostra i problemi del file audio (se ce ne sono):
```shell
afinfo --warnings {{percorso/del/file}}
```
#### Mostra la pagina di aiuto:
```shell
afinfo -h
```
{% endraw %}