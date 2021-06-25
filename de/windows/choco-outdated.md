---
layout: default
title: "choco outdated"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-outdated">
  <a href="/de/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Überprüfe mit Chocolatey, ob Pakete veraltet sind.
> Weitere Informationen: <https://chocolatey.org/docs/commands-outdated>.

#### Zeige eine Liste von veralteten Paketen im Tabellen-Format:
```shell
choco outdated
```
#### Ignoriere angeheftete Pakete in der Ausgabe:
```shell
choco outdated --ignore-pinned
```
#### Gib eine eigene Quelle an, mit der die Aktualität der Pakete überprüft wird:
```shell
choco outdated --source {{source_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco outdated --user {{benutzername}} --password {{passwort}}
```
{% endraw %}