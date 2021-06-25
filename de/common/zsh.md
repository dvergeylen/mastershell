---
layout: default
title: "zsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zsh">
  <a href="/de/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell.
> Mit `bash` und `sh` kompatible Eingabeaufforderung.
> Weitere Informationen: <https://www.zsh.org>.

#### Starte eine interaktive Eingabeaufforderung:
```shell
zsh
```
#### Führe Parameter als Befehl aus:
```shell
zsh -c {{befehl}}
```
#### Führe Befehle aus einem Skript aus:
```shell
zsh {{pfad/zu/skript}}
```
#### Führe Befehle aus einem Skript aus und schreibe die Befehle in die Konsole:
```shell
zsh --xtrace {{pfad/zu/skript}}
```
#### Starte eine interaktive Eingabeaufforderung, in der jeder Befehl ausgegeben wird, bevor er ausgeführt wird:
```shell
zsh --verbose
```
{% endraw %}