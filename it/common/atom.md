---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/it/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un editor di testo cross-platform personalizzabile.
> I plugin sono gestiti da `apm`.
> Maggiori informazioni: <https://atom.io/>.

#### Apri un file o una cartella:
```shell
atom {{percorso/a/file_o_cartella}}
```
#### Apri un file o una cartella in una nuova finestra:
```shell
atom -n {{percorso/a/file_o_cartella}}
```
#### Apri un file o una cartella in una finestra esistente:
```shell
atom --add {{percorso/a/file_o_cartella}}
```
#### Avvia Atom in safe mode (non carica nessun pacchetto):
```shell
atom --safe
```
#### Impedisci ad Atom di creare un nuovo processo in background, lasciandolo in esecuzione nel terminale:
```shell
atom --foreground
```
{% endraw %}