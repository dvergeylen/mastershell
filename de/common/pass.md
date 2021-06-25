---
layout: default
title: "pass"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pass">
  <a href="/de/common/pass.html">pass</a> <a href="#pass"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Programm zum Speichern und Lesen von Passwörtern und anderen sensiblen Daten.
> Die Daten sind mit GPG verschlüsselt und werden mit einem Git repository verwaltet.
> Weitere Informationen: <https://www.passwordstore.org>.

#### Initialisiere oder verschlüssle einen neuen oder bestehenden Speicher mit einer oder mehreren GPG IDs neu:
```shell
pass init {{gpg_id_1}} {{gpg_id_2}}
```
#### Speichere das Passwort und zusätzliche Informationen (Str + D auf neuer Zeile zum abschließen):
```shell
pass insert --multiline {{pfad/zu/datei}}
```
#### Bearbeite einen bestimmten Eintrag:
```shell
pass edit {{pfad/zu/datei}}
```
#### Kopiere das Passwort (die erste Zeile des Eintrags) in die Zwischenablage:
```shell
pass -c {{pfad/zu/datei}}
```
#### Zeige die Baumstruktur des Passwort-Stores an:
```shell
pass
```
#### Generiere ein neues, zufälliges Passwort mit Länge n und kopiere is in die Zwischenablage:
```shell
pass generate -c {{pfad/zu/datei}} {{n}}
```
#### Initialisiere ein Git Repository (Alle durch pass durchgeführten Änderungen werden automatisch committed):
```shell
pass git init
```
{% endraw %}