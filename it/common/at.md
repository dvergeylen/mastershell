---
layout: default
title: "at"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="at">
  <a href="/it/common/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programma l'esecuzione di comandi nel futuro.
> Il servizio atd (o atrun) deve essere attivo per eseguire i comandi.
> Maggiori informazioni: <https://man.archlinux.org/man/at.1>.

#### Esegui i comandi inseriti standard input tra 5 minuti (premere `Ctrl + D` dopo aver inserito i comandi):
```shell
at now + 5 minutes
```
#### Esegui un comando passato da standard input alle 10:00 di mattina:
```shell
echo "{{./mio_script.sh}}" | at 1000
```
#### Esegui comandi contenuti in un dato file il prossimo martedì alle 9:30 di sera:
```shell
at -f {{percorso/al/file}} 9:30 PM Tue
```
{% endraw %}