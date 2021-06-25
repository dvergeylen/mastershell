---
layout: default
title: "steam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="steam">
  <a href="/en/common/steam.html">steam</a> <a href="#steam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Video game platform by Valve.
> More information: <https://developer.valvesoftware.com/wiki/Command_Line_Options#Steam_.28Windows.29>.

#### Launch Steam, printing debug messages to stdout:
```shell
steam
```
#### Launch Steam and enable its in-app debug console tab:
```shell
steam -console
```
#### Log into Steam with the specified credentials:
```shell
steam -login {{username}} {{password}}
```
#### Launch Steam in Big Picture Mode:
```shell
steam -tenfoot
```
#### Exit Steam:
```shell
steam -shutdown
```
{% endraw %}