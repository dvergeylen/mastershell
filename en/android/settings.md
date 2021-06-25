---
layout: default
title: "settings"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="settings">
  <a href="/en/android/settings.html">settings</a> <a href="#settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get information about the Android OS.
> More information: <https://adbinstaller.com/commands/adb-shell-settings-5b670d5ee7958178a2955536>.

#### Display a list of settings in the `global` namespace:
```shell
settings list {{global}}
```
#### Get the value of a specific setting:
```shell
settings get {{global}} {{airplane_mode_on}}
```
#### Set the value of a setting:
```shell
settings put {{system}} {{screen_brightness}} {{42}}
```
#### Delete a specific setting:
```shell
settings delete {{secure}} {{screensaver_enabled}}
```
{% endraw %}