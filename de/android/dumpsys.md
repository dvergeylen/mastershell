---
layout: default
title: "dumpsys"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dumpsys">
  <a href="/de/android/dumpsys.html">dumpsys</a> <a href="#dumpsys"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Stelle Informationen über Android-Systemservices bereit.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://developer.android.com/studio/command-line/dumpsys>.

#### Erhalte diagnostische Informationen über alle Systemservices:
```shell
dumpsys
```
#### Erhalte diagnostische Informationen über einen bestimmten Systemservice:
```shell
dumpsys {{service}}
```
#### Liste alle Services, über die `dumpsys` Informationen bereitstellen kann auf:
```shell
dumpsys -l
```
#### Liste Service-spezifische Argumente für einen Service auf:
```shell
dumpsys {{service}} -h
```
#### Schließe einen bestimmten Service von den diagnostischen Informationen aus:
```shell
dumpsys --skip {{service}}
```
#### Gib ein Timeout in Sekunden an (standardmäßig 10s):
```shell
dumpsys -t {{sekunden}}
```
{% endraw %}