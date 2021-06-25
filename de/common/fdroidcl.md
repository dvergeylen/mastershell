---
layout: default
title: "fdroidcl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdroidcl">
  <a href="/de/common/fdroidcl.html">fdroidcl</a> <a href="#fdroidcl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid CLI (Command-line Interface) Client.
> Weitere Informationen: <https://github.com/mvdan/fdroidcl>.

#### Aktualisiere den Index:
```shell
fdroidcl update
```
#### Zeige Informationen über eine App:
```shell
fdroidcl show {{app_id}}
```
#### Lade eine apk-Datei herunter:
```shell
fdroidcl download {{app_id}}
```
#### Suche nach einer App im Index:
```shell
fdroidcl search {{suchmuster}}
```
#### Installiere eine App auf einem verbundenen Gerät:
```shell
fdroidcl install {{app_id}}
```
{% endraw %}