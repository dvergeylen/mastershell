---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/it/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rimuovi file o directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/rm>.

#### Rimuovi file:
```shell
rm {{percorso/a/file1 percorso/a/file2 ...}}
```
#### Rimuovi ricorsivamente una directory e tutti i suoi contenuti:
```shell
rm -r {{percorso/alla/directory}}
```
#### Rimuovi ricorsivamente una directory, senza chiedere conferma o mostrare messaggi di errore:
```shell
rm -rf {{percorso/alla/directory}}
```
#### Rimuovi file interattivamente, chiedendo conferma prima di rimuovere ogni file:
```shell
rm -i {{file(s)}}
```
#### Rimuovi file in modalità verbosa, scrivendo un messaggio a schermo per ogni file rimosso:
```shell
rm -v {{percorso/a/un/file}}
```
{% endraw %}