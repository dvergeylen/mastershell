---
layout: default
title: "cradle package"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-package">
  <a href="/de/common/cradle-package.html">cradle package</a> <a href="#cradle-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Pakete für Cradle Instanzen.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#package>.

#### Liste aller verfügbaren Pakete auf:
```shell
cradle package list
```
#### Suche nach einem Paket:
```shell
cradle package search {{paket}}
```
#### Installiere ein Paket von Packagist:
```shell
cradle package install {{paket}}
```
#### Installiere eine bestimmte Version eines Pakets:
```shell
cradle package install {{paket}} {{version}}
```
#### Aktualisiere eine Paket:
```shell
cradle package update {{paket}}
```
#### Aktualisiere ein Paketes zu einer bestimmten Paket-Version:
```shell
cradle package update {{paket}} {{version}}
```
#### Entferne eine Paket:
```shell
cradle package remove {{paket}}
```
{% endraw %}