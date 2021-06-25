---
layout: default
title: "fish"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fish">
  <a href="/de/common/fish.html">fish</a> <a href="#fish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Friendly Interactive SHell.
> Eine benutzerfreundliche Eingabeaufforderung.
> Weitere Informationen: <https://fishshell.com>.

#### Starte eine interaktive Shell-Sitzung:
```shell
fish
```
#### Führe einen Befehl aus:
```shell
fish -c "{{befehl}}"
```
#### Führe ein Skript aus:
```shell
fish {{pfad/zu/skript.fish}}
```
#### Überprüfe ein Skript auf Syntaxfehler:
```shell
fish --no-execute {{pfad/zu/skript.fish}}
```
#### Starte eine private interaktive Shell-Sitzung, in der `fish` weder auf die Shell-History zugreift, noch diese verändert:
```shell
fish --private
```
#### Gib die Version von fish aus:
```shell
fish --version
```
#### Setze und exportiere eine permanente Umgebungsvariable (nur innerhalb der Shell):
```shell
set -Ux {{variablenname}} {{variablenwert}}
```
{% endraw %}