---
layout: default
title: "bower"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bower">
  <a href="/it/common/bower.html">bower</a> <a href="#bower"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un manager di pacchetti ottimizzato per sviluppo web front-end.
> Un pacchetto può essere una abbreviazione utente/repo GitHub, un endpoint Git, un URL o un pacchetto registrato.
> Maggiori informazioni: <https://bower.io/>.

#### Installa le dipendenze di un progetto, listate nel suo file `bower.json`:
```shell
bower install
```
#### Installa pacchetti nella directory bower_components:
```shell
bower install {{pacchetto1}} {{pacchetto2}} ...
```
#### Disinstalla pacchetti localmente rimuovendolo dalla directory bower_components:
```shell
bower uninstall {{pacchetto1}} {{pacchetto2}}
```
#### Elenca pacchetti locali e possibili aggiornamenti:
```shell
bower list
```
#### Mostra aiuto per un comando di bower:
```shell
bower help {{comando}}
```
#### Crea un file bower.json per i tuoi pacchetti:
```shell
bower init
```
#### Installa unoa specifica versione di una dipendenza ed aggiungila al file `bower.json`:
```shell
bower install {{nome_locale}}={{pacchetto}}#{{versione}} --save
```
{% endraw %}