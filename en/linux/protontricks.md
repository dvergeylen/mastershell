---
layout: default
title: "protontricks"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="protontricks">
  <a href="/en/linux/protontricks.html">protontricks</a> <a href="#protontricks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple wrapper that does Winetricks things for Proton enabled games, requires Winetricks.
> More information: <https://github.com/Matoking/protontricks>.

#### Show the protontricks help message:
```shell
protontricks
```
#### Run the protontricks GUI:
```shell
protontricks --gui
```
#### Run Winetricks for a specific game:
```shell
protontricks {{appid}} {{winetricks_args}}
```
#### Run a command within a games installation directory:
```shell
protontricks -c {{command}} {{appid}}
```
{% endraw %}