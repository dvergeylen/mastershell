---
layout: default
title: "bugreportz"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bugreportz">
  <a href="/de/android/bugreportz.html">bugreportz</a> <a href="#bugreportz"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiere einen gezippten Android-Fehlerbericht.
> Dieser Befehl kann nur mit `adb shell` verwendet werden.
> Weitere Informationen: <https://android.googlesource.com/platform/frameworks/native/+/master/cmds/bugreportz/>.

#### Generiere einen vollständigen Fehlerbericht eines Android Geräts:
```shell
bugreportz
```
#### Zeige den Fortschritt eines laufenden `bugreportz` Prozesses an:
```shell
bugreportz -p
```
#### Zeige die Versionsnummer von `bugreportz` an:
```shell
bugreportz -v
```
#### Zeige Hilfe an:
```shell
bugreportz -h
```
{% endraw %}