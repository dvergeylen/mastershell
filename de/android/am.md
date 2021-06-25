---
layout: default
title: "am"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="am">
  <a href="/de/android/am.html">am</a> <a href="#am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Androids Aktivitäten-Manager.
> Weitere Informationen: <https://developer.android.com/studio/command-line/adb#am>.

#### Starte eine bestimmte Aktivität:
```shell
am start -n {{com.android.settings/.Settings}}
```
#### Starte eine Aktivität und übergib ihr Daten:
```shell
am start -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
#### Starte eine Aktivität, auf die eine bestimmte Aktion und Kategorie zutrifft:
```shell
am start -a {{android.intent.action.MAIN}} -c {{android.intent.category.HOME}}
```
#### Konvertiere ein bestimmtes Ziel in einen URI:
```shell
am to-uri -a {{android.intent.action.VIEW}} -d {{tel:123}}
```
{% endraw %}