---
layout: default
title: "choco-apikey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-apikey">
  <a href="/de/windows/choco-apikey.html">choco-apikey</a> <a href="#choco-apikey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte die API-Schlüssel für die Quellen von Chocolatey.
> Weitere Informationen: <https://chocolatey.org/docs/commands-apikey>.

#### Gib eine Liste von Quellen und ihren API-Schlüsseln aus:
```shell
choco apikey
```
#### Zeige eine bestimmte Quelle und ihren API-Schlüssel an:
```shell
choco apikey --source "{{quell_url}}"
```
#### Setze den API-Schlüssel für eine Quelle:
```shell
choco apikey --source "{{quell_url}}" --key "{{api_schluessel}}"
```
#### Entferne den API-Schlüssel einer Quelle:
```shell
choco apikey --source "{{quell_url}}" --remove
```
{% endraw %}