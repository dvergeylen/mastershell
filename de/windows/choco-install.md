---
layout: default
title: "choco install"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-install">
  <a href="/de/windows/choco-install.html">choco install</a> <a href="#choco-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Installiere ein oder mehrere Pakete mit Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-install>.

#### Installiere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco install {{paket1}} {{paket2}}
```
#### Installiere Pakete aus einer Konfigurationsdatei:
```shell
choco install {{pfad/zu/pakete.config}}
```
#### Installiere Pakete aus einer `nuspec`- oder `nupkg`-Datei:
```shell
choco install {{pfad/zu/datei}}
```
#### Installiere eine bestimmte Version eines Pakets:
```shell
choco install {{paket}} --version {{version}}
```
#### Erlaube die gleichzeitige Installation mehrerer Versionen eines Pakets:
```shell
choco install {{paket}} --allow-multiple
```
#### Stimme allen Fragen automatisch zu:
```shell
choco install {{paket}} --yes
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco install {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco install {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}