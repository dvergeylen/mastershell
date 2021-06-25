---
layout: default
title: "pm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pm">
  <a href="/de/android/pm.html">pm</a> <a href="#pm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zeige Informationen über Apps auf einem Android Gerät.
> Weitere Informationen: <https://developer.android.com/studio/command-line/adb#pm>.

#### Gib eine Liste aller installierten Apps aus:
```shell
pm list packages
```
#### Gib eine Liste aller installierten System-Apps aus:
```shell
pm list packages -s
```
#### Gib eine Liste aller installierten Apps von Drittanbietern aus:
```shell
pm list packages -3
```
#### Gib eine Liste aller Apps, auf die ein bestimmtes Schlüsselwort zutrifft, aus:
```shell
pm list packages {{Schlüsselwort}}
```
#### Gib den Pfad der APK einer bestimmten App aus:
```shell
pm path {{app}}
```
{% endraw %}