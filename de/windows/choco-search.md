---
layout: default
title: "choco search"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-search">
  <a href="/de/windows/choco-search.html">choco search</a> <a href="#choco-search"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Suche mit Chocolatey nach einem lokal oder im Internet verfügbaren Paket.
> Weitere Informationen: <https://chocolatey.org/docs/commands-search>.

#### Suche nach einem Paket:
```shell
choco search {{suchabfrage}}
```
#### Suche nur lokal nach einem Paket:
```shell
choco search {{suchabfrage}} --local-only
```
#### Suche nur nach genauen Übereinstimmungen:
```shell
choco search {{suchabfrage}} --exact
```
#### Stimme allen Fragen automatisch zu:
```shell
choco search {{suchabfrage}} --yes
```
#### Gib eine eigene Quelle an, welche nach Paketen durchsucht wird:
```shell
choco search {{suchabfrage}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco search {{suchabfrage}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}