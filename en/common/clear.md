---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/en/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clears the screen of the terminal.
> More information: <https://manned.org/clear>.

#### Clear the screen (equivalent to pressing Control-L in Bash shell):
```shell
clear
```
#### Clear the screen but keep the terminal's scrollback buffer:
```shell
clear -x
```
#### Indicate the type of terminal to clean (defaults to the value of the environment variable `TERM`):
```shell
clear -T {{type_of_terminal}}
```
#### Show the version of `ncurses` used by `clear`:
```shell
clear -V
```
{% endraw %}