---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/de/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Erstellt Aliasse - Alterative Namen für Befehle.
> Aliasse laufen mit der aktuellen Shell-Sitzung ab, es sei denn, sie werden in der Konfigurationsdatei der Shell definiert, z.B. `~/.bashrc`.
> Weitere Informationen: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listet alle Aliasse auf:
```shell
alias
```
#### Erstellt einen Alias:
```shell
alias {{alias}}="{{befehl}}"
```
#### Zeigt den mit einem bestimmten Alias verknüpften Befehl an:
```shell
alias {{alias}}
```
#### Entferne einen Alias:
```shell
unalias {{alias}}
```
#### Macht `rm` zu einem interaktiven Befehl:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Erstellt den Alias `la` für `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}