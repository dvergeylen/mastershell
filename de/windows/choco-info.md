---
layout: default
title: "choco info"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-info">
  <a href="/de/windows/choco-info.html">choco info</a> <a href="#choco-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige ausführliche Informationen über ein Chocolatey-Paket an.
> Weitere Informationen: <https://chocolatey.org/docs/commands-info>.

#### Zeige Informationen über ein bestimmtes Paket an:
```shell
choco info {{paket}}
```
#### Zeige Informationen über ein bestimmtes lokales Paket an:
```shell
choco info {{paket}} --local-only
```
#### Gib eine eigene Quelle an, von der Paket-Informationen abgerufen werden:
```shell
choco info {{paket}} --source {{quell_url|alias}}
```
#### Gib einen Benutzernamen und ein Passwort für die Authentifizierung an:
```shell
choco info {{paket}} --user {{benutzername}} --password {{passwort}}
```
{% endraw %}