---
layout: default
title: "logcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="logcat">
  <a href="/de/android/logcat.html">logcat</a> <a href="#logcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gib ein Protokoll aller Systemmeldungen aus:
> Weitere Informationen: <https://developer.android.com/studio/command-line/logcat>.

#### Gib ein Protokoll aller Systemmeldungen aus:
```shell
logcat
```
#### Schreibe alle Systemmeldungen in eine Datei:
```shell
logcat -f {{pfad/zu/datei}}
```
#### Gib Zeilen aus, die einem regulären Ausdruck entsprechen:
```shell
logcat --regex {{regex}}
```
{% endraw %}