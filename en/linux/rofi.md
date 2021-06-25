---
layout: default
title: "rofi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rofi">
  <a href="/en/linux/rofi.html">rofi</a> <a href="#rofi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An application launcher and window switcher.
> More information: <https://github.com/davatorium/rofi>.

#### Show the list of apps:
```shell
rofi -show drun
```
#### Show the list of all commands:
```shell
rofi -show run
```
#### Switch between windows:
```shell
rofi -show window
```
#### Pipe a list of items to stdin and print the selected item to stdout:
```shell
printf "{{Choice1\nChoice2\nChoice3}}" | rofi -dmenu
```
{% endraw %}