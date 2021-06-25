---
layout: default
title: "choco upgrade"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-upgrade">
  <a href="/de/windows/choco-upgrade.html">choco upgrade</a> <a href="#choco-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aktualisiere mit Chocolatey ein oder mehrere Pakete.
> Weitere Informationen: <https://chocolatey.org/docs/commands-upgrade>.

#### Aktualisiere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco upgrade {{paket(e)}}
```
#### Aktualisiere auf eine bestimmte Version des Pakets:
```shell
choco upgrade {{paket}} --version {{version}}
```
#### Aktualisiere alle Pakete:
```shell
choco upgrade all
```
#### Aktualisiere alle außer den angegebenen, durch Kommas getrennten Paketen:
```shell
choco upgrade all --except "{{paket(e)}}"
```
#### Stimme allen Fragen automatisch zu:
```shell
choco upgrade {{paket}} --yes
```
#### Gib eine eigene Quelle an, von der Pakete aktualisiert werden:
```shell
choco upgrade {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco upgrade {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}