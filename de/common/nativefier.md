---
layout: default
title: "nativefier"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nativefier">
  <a href="/de/common/nativefier.html">nativefier</a> <a href="#nativefier"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Befehlszeilen-Tool zum Erstellen einer Desktop-Anwendung für jede Website mit minimaler Konfiguration.
> Weitere Informationen: <https://github.com/jiahaog/nativefier>.

#### Erstelle einer Desktop-Anwendung für eine Website:
```shell
nativefier {{url}}
```
#### Erstelle eine Desktop-Anwendung mit einem benutzerdefinierten Namen:
```shell
nativefier --name {{name}} {{url}}
```
#### Verwende ein benutzerdefiniertes Icon:
```shell
nativefier --icon {{pfad/zu/icon.png}} {{url}}
```
{% endraw %}