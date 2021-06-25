---
layout: default
title: "fdroid"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fdroid">
  <a href="/de/common/fdroid.html">fdroid</a> <a href="#fdroid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> F-Droid Build Tool.
> F-Droid ist ein installierbarer Katalog mit FOSS (Freie Open Source Software) Apps für Android.
> Weitere Informationen: <https://f-droid.org/>.

#### Kompiliere eine bestimmte App:
```shell
fdroid build {{app_id}}
```
#### Kompiliere eine bestimmte App in einer Build-Server-VM:
```shell
fdroid build {{app_id}} --server
```
#### Veröffentliche die App im lokalen Repository:
```shell
fdroid publish {{app_id}}
```
#### Installiere die App auf jedem verbundenen Gerät:
```shell
fdroid install {{app_id}}
```
#### Überprüfe, ob die Metadaten korrekt formatiert sind:
```shell
fdroid lint --format {{app_id}}
```
#### Korrigiere die Formatierung automatisch (wenn möglich):
```shell
fdroid rewritemeta {{app_id}}
```
{% endraw %}