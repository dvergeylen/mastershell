---
layout: default
title: "lxterminal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lxterminal">
  <a href="/en/linux/lxterminal.html">lxterminal</a> <a href="#lxterminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal emulator for LXDE.
> More information: <https://wiki.lxde.org/en/LXTerminal>.

#### Open an LXTerminal window:
```shell
lxterminal
```
#### Open an LXTerminal window, run a command, and then exit:
```shell
lxterminal -e "{{command}}"
```
#### Open an LXTerminal window with multiple tabs:
```shell
lxterminal --tabs={{tab_name1,tab_name2,...}}
```
#### Open an LXTerminal window with a specific title:
```shell
lxterminal --title={{title_name}}
```
#### Open an LXTerminal window with a specific working directory:
```shell
lxterminal --working-directory={{path/to/directory}}
```
{% endraw %}