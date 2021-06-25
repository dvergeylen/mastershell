---
layout: default
title: "choco uninstall"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-uninstall">
  <a href="/de/windows/choco-uninstall.html">choco uninstall</a> <a href="#choco-uninstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deinstalliere mit Chocolatey ein oder mehrere Pakete.
> Weitere Informationen: <https://chocolatey.org/docs/commands-uninstall>.

#### Deinstalliere ein oder mehrere Pakete, deren Namen mit Leerzeichen getrennt sind:
```shell
choco uninstall {{paket(e)}}
```
#### Deinstalliere eine bestimmte Version eines Paketes:
```shell
choco uninstall {{paket}} --version {{version}}
```
#### Stimme allen Fragen automatisch zu:
```shell
choco uninstall {{paket}} --yes
```
#### Deinstalliere auch alle Abhängigkeiten:
```shell
choco uninstall {{paket}} --remove-dependencies
```
#### Deinstalliere alle Pakete:
```shell
choco uninstall all
```
{% endraw %}