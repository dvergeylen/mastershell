---
layout: default
title: "git"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git">
  <a href="/de/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verteiltes Versionskontrollsystem.
> Weitere Informationen: <https://git-scm.com/>.

#### Gib die installierte Git Version aus:
```shell
git --version
```
#### Zeige die generelle Hilfsseite an:
```shell
git --help
```
#### Zeige die Hilfsseite eines Unterbefehls an:
```shell
git help {{unterbefehl}}
```
#### Führe einen Git-Unterbefehl aus:
```shell
git {{unterbefehl}}
```
#### Führe einen Git-Unterbefehl auf einem benutzerdefinierten Repository aus:
```shell
git -C {{pfad/zu/repository}} {{unterbefehl}}
```
#### Führe einen Git-Unterbefehl mit der angegebenen Konfiguration aus:
```shell
git -c '{{config.key}}={{wert}}' {{unterbefehl}}
```
{% endraw %}