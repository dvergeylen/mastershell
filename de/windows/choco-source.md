---
layout: default
title: "choco source"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-source">
  <a href="/de/windows/choco-source.html">choco source</a> <a href="#choco-source"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte die Paketquellen mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-source>.

#### Gib alle momentan verfügbaren Quellen aus:
```shell
choco source list
```
#### Füge eine neue Paketquelle hinzu:
```shell
choco source add --name {{name}} --source {{url}}
```
#### Füge eine neue Paketquelle mit Zugangsdaten hinzu:
```shell
choco source add --name {{name}} --source {{url}} --user {{benutzername}} --password {{passwort}}
```
#### Füge eine neue Paketquelle mit Client-Zertifikat hinzu:
```shell
choco source add --name {{name}} --source {{url}} --cert {{pfad/zu/zertifikat}}
```
#### Aktiviere eine Paketquelle:
```shell
choco source enable --name {{name}}
```
#### Deaktiviere eine Paketquelle:
```shell
choco source disable --name {{name}}
```
#### Entferne eine Paketquelle:
```shell
choco source remove --name {{name}}
```
{% endraw %}