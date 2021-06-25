---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/de/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> `sh`-kompatibler Kommandozeilen-Interpreter.
> Weitere Informationen: <https://gnu.org/software/bash>.

#### Interaktive Shell starten:
```shell
bash
```
#### Führe einen Befehl aus:
```shell
bash -c "{{befehl}}"
```
#### Führe Befehle aus einer Datei aus:
```shell
bash {{pfad/zu/datei.sh}}
```
#### Führe Befehle aus einer Datei aus and protokolliere alle ausgeführten Befehle an das Terminal:
```shell
bash -x {{pfad/zu/datei.sh}}
```
#### Führe Befehle aus einer Datei aus und stoppe beim ersten Fehler:
```shell
bash -e {{pfad/zu/datei.sh}}
```
#### Führe Befehle von stdin aus:
```shell
bash -s
```
#### Gib die Version von bash aus (verwende `echo $BASH_VERSION`, um nur die Versionszeichenkette anzuzeigen):
```shell
bash --version
```
{% endraw %}