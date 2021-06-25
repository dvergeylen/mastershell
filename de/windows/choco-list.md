---
layout: default
title: "choco list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-list">
  <a href="/de/windows/choco-list.html">choco list</a> <a href="#choco-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige mit Chocolatey eine Liste von Paketen an.
> Weitere Informationen: <https://chocolatey.org/docs/commands-list>.

#### Zeige alle verfügbaren Pakete an:
```shell
choco list
```
#### Zeige alle lokal installierten Pakete an:
```shell
choco list --local-only
```
#### Zeige eine Liste einschließlich der lokalen Windows-Programme an:
```shell
choco list --include-programs
```
#### Zeige nur zugelassene Pakete an:
```shell
choco list --approved-only
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco list --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco list --user {{benutzername}} --password {{passwort}}
```
{% endraw %}