---
layout: default
title: "kwriteconfig5"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="kwriteconfig5">
  <a href="/en/linux/kwriteconfig5.html">kwriteconfig5</a> <a href="#kwriteconfig5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write KConfig entries for KDE Plasma.
> More information: <https://userbase.kde.org/KDE_System_Administration/Configuration_Files>.

#### Display help:
```shell
kwriteconfig5 --help
```
#### Set a global configuration key:
```shell
kwriteconfig5 --group {{group_name}} --key {{key}} {{value}}
```
#### Set a key in a specific configuration file:
```shell
kwriteconfig5 --file {{path/to/file}} --group {{group_name}} --key {{key}} {{value}}
```
#### Delete a key:
```shell
kwriteconfig5 --group {{group_name}} --key {{key}} --delete
```
#### Use systemd to start the Plasma session when available:
```shell
kwriteconfig5 --file {{startkderc}} --group {{General}} --key {{systemdBoot}} {{true}}
```
#### Hide the title bar when a window is maximized (like Ubuntu):
```shell
kwriteconfig5 --file {{~/.config/kwinrc}} --group {{Windows}} --key {{BorderlessMaximizedWindows}} {{true}}
```
#### Configure KRunner to open with the Meta (Command/Windows) global hotkey:
```shell
kwriteconfig5 --file {{~/.config/kwinrc}} --group {{ModifierOnlyShortcuts}} --key {{Meta}} {{"org.kde.kglobalaccel,/component/krunner_desktop,org.kde.kglobalaccel.Component,invokeShortcut,_launch"}}
```
{% endraw %}