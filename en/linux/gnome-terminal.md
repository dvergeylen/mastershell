---
layout: default
title: "gnome-terminal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gnome-terminal">
  <a href="/en/linux/gnome-terminal.html">gnome-terminal</a> <a href="#gnome-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The GNOME Terminal emulator.

#### Open a new GNOME terminal window:
```shell
gnome-terminal
```
#### Run a specific command in a new terminal window:
```shell
gnome-terminal -- {{command}}
```
#### Open a new tab in the last opened window instead:
```shell
gnome-terminal --tab
```
#### Set the title of the new tab:
```shell
gnome-terminal --tab --title "{{title}}"
```
{% endraw %}