---
layout: default
title: "batch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="batch">
  <a href="/it/common/batch.html">batch</a> <a href="#batch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui comandi nel futuro quando il carico di lavoro del sistema lo permette.
> Il servizio atd (o atrun) deve essere attivo per eseguire i comandi.
> Maggiori informazioni: <https://man.archlinux.org/man/at.1>.

#### Esegui i comandi inseriti standard input (premere `Ctrl + D` dopo aver inserito i comandi):
```shell
batch
```
#### Esegui un comando da standard input:
```shell
echo "{{./mio_script.sh}}" | batch
```
#### Esegui comandi contenuti in un dato file:
```shell
batch -f {{percorso/al/file}}
```
{% endraw %}