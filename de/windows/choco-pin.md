---
layout: default
title: "choco pin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pin">
  <a href="/de/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hefte ein Chocolatey-Paket bei einer bestimmten Version an.
> Angeheftete Pakete werden nicht weiter aktualisiert.
> Weitere Informationen: <https://chocolatey.org/docs/commands-pin>.

#### Zeige eine Liste der angehefteten Pakete und ihrer Versionen an:
```shell
choco pin list
```
#### Hefte ein Paket in der installierten Version an:
```shell
choco pin add --name {{paket}}
```
#### Hefte ein Paket in einer bestimmten Version an:
```shell
choco pin add --name {{paket}} --version {{version}}
```
#### Entferne die Anheftung für ein bestimmtes Paket:
```shell
choco pin remove --name {{paket}}
```
{% endraw %}