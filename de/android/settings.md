---
layout: default
title: "settings"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="settings">
  <a href="/de/android/settings.html">settings</a> <a href="#settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Verwalte Android-Systemeinstellungen.
> Weitere Informationen: <https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

#### Gib eine Liste aller Einstellungen im Namespace `global` aus:
```shell
settings list {{global}}
```
#### Gib den Wert einer bestimmten Einstellung aus:
```shell
settings get {{global}} {{airplane_mode_on}}
```
#### Setze den Wert einer bestimmten Einstellung:
```shell
settings put {{system}} {{screen_brightness}} {{42}}
```
#### Lösche eine bestimmte Einstellung:
```shell
settings delete {{secure}} {{screensaver_enabled}}
```
{% endraw %}