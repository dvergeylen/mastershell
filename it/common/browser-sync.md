---
layout: default
title: "browser-sync"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="browser-sync">
  <a href="/it/common/browser-sync.html">browser-sync</a> <a href="#browser-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Avvia un web-server locale che si aggiorna al cambiamento dei file.
> Maggiori informazioni: <https://browsersync.io/docs/command-line>.

#### Avvia un server da una specifica directory:
```shell
browser-sync start --server {{percorso/a/directory}} --files {{percorso/a/directory}}
```
#### Avvia un server da una directory locale, monitorando tutti i file CSS:
```shell
browser-sync start --server --files '{{percorso/a/directory/*.css}}'
```
#### Crea un file di configurazione:
```shell
browser-sync init
```
#### Avvia bower-sync da un file di configurazione:
```shell
browser-sync start --config {{file_di_configurazione}}
```
{% endraw %}