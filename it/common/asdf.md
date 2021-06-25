---
layout: default
title: "asdf"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asdf">
  <a href="/it/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaccia da linea di comando per gestire le versionai di diversi pacchetti.
> Maggiori informazioni: <https://asdf-vm.com>.

#### Elenca tutti i plugin disponibili:
```shell
asdf plugin-list-all
```
#### Installa un plugin:
```shell
asdf plugin-add {{nome}}
```
#### Elenca tutte le versioni disponibili per un pacchetto:
```shell
asdf list-all {{nome}}
```
#### Installa una specifica versione di un pacchetto:
```shell
asdf install {{nome}} {{versiona}}
```
#### Imposta la versione globale per un pacchetto:
```shell
asdf global {{nome}} {{versiona}}
```
#### Imposta la versiona locale per un pacchetto:
```shell
asdf local {{nome}} {{versiona}}
```
{% endraw %}