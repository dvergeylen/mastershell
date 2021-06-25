---
layout: default
title: "pio settings"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-settings">
  <a href="/en/common/pio-settings.html">pio settings</a> <a href="#pio-settings"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View and modify PlatformIO settings.
> More information: <https://docs.platformio.org/en/latest/core/userguide/cmd_settings.html>.

#### Display the names, values and descriptions of all PlatformIO settings:
```shell
pio settings get
```
#### Display the name, value and description of a specific PlatformIO setting:
```shell
pio settings get {{setting}}
```
#### Set a specific setting value:
```shell
pio settings set {{setting}} {{value}}
```
#### Reset the values of all modified settings to their factory defaults:
```shell
pio settings reset
```
{% endraw %}