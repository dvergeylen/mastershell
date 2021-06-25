---
layout: default
title: "cradle install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cradle-install">
  <a href="/de/common/cradle-install.html">cradle install</a> <a href="#cradle-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere Cradle PHP Framework Komponenten.
> Weitere Informationen: <https://cradlephp.github.io/docs/3.B.-Reference-Command-Line-Tools.html#install>.

#### Installiere Cradle Komponenten mithilfe eines Dialogs:
```shell
cradle install
```
#### Installiere Cradle Komponenten gewaltsam:
```shell
cradle install --force
```
#### Überspringe SQL Migrationen:
```shell
cradle install --skip-sql
```
#### Überspringe Paket-Aktualisierungen:
```shell
cradle install --skip-versioning
```
#### Zeige Details über eine benutzer-spezifische Datenbank:
```shell
cradle install -h {{hostname}} -u {{benutzer}} -p {{passwort}}
```
{% endraw %}