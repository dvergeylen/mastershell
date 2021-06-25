---
layout: default
title: "ffsend"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ffsend">
  <a href="/de/common/ffsend.html">ffsend</a> <a href="#ffsend"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Teile Dateien einfach und sicher in der Command-line.
> Weitere Informationen: <https://gitlab.com/timvisee/ffsend>.

#### Lade eine Datei hoch:
```shell
ffsend upload {{datei}}
```
#### Lade eine Datei herunter:
```shell
ffsend download {{url}}
```
#### Lade eine Datei mit Passwort hoch:
```shell
ffsend upload {{datei}} -p {{passwort}}
```
#### Lade eine passwortgeschützte Datei herunter:
```shell
ffsend download {{datei}} -p {{passwort}}
```
#### Lade eine Datei hoch und erlaube maximal 4 Downloads:
```shell
ffsend upload {{datei}} -d {{4}}
```
{% endraw %}