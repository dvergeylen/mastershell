---
layout: default
title: "borg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="borg">
  <a href="/it/common/borg.html">borg</a> <a href="#borg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Strumento di backup con deduplicazione.
> Crea backup locali o remoti che sono montabili come filesystem.
> Maggiori informazioni: <https://borgbackup.readthedocs.io/en/stable/usage/general.html>.

#### Inizializza una repository (locale):
```shell
borg init {{/percorso/a/repo_o_directory}}
```
#### Esegui il backup di una directory nella repository, creando un archivio chiamato "Lunedi":
```shell
borg create --progress {{/percorso/a/repo_o_directory}}::{{Lunedi}} {{/percorso/a/directory_sorgente}}
```
#### Lista tutti gli archivi in una repository:
```shell
borg list {{/percorso/a/repo_o_directory}}
```
#### Estrai una specifica directory dall'archivio "Lunedi" in una repository remota, escludendo tutti i file `.ext`:
```shell
borg extract {{utente}}@{{host}}:{{/percorso/a/repo_o_directory}}::{{Lunedi}} {{percorso/a/cartella_destinazione}} --exclude '{{*.ext}}'
```
#### Riduci una repository eliminando tutti gli archivi più vecchi di 7 giorni, elencando i cambiamenti:
```shell
borg prune --keep-within {{7d}} --list {{/percorso/a/repo_o_directory}}
```
#### Monta una repository come filesystem FUSE:
```shell
borg mount {{/percorso/a/repo_o_directory}}::{{Lunedi}} {{/percorso/a/mountpoint}}
```
#### Mostra aiuto sul come creare archivi:
```shell
borg create --help
```
{% endraw %}