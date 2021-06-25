---
layout: default
title: "xfce4-terminal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xfce4-terminal">
  <a href="/en/linux/xfce4-terminal.html">xfce4-terminal</a> <a href="#xfce4-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The XFCE4 terminal emulator.
> More information: <https://docs.xfce.org/apps/xfce4-terminal/start>.

#### Open a new terminal window:
```shell
xfce4-terminal
```
#### Set the initial title:
```shell
xfce4-terminal --initial-title "{{initial_title}}"
```
#### Open a new tab in the current terminal window:
```shell
xfce4-terminal --tab
```
#### Execute a command in a new terminal window:
```shell
xfce4-terminal --command "{{command_with_args}}"
```
#### Keep the terminal around after the executed command finishes executing:
```shell
xfce4-terminal --command "{{command_with_args}}" --hold
```
#### Open multiple new tabs, executing a command in each:
```shell
xfce4-terminal --tab --command "{{command_a}}" --tab --command "{{command_b}}"
```
{% endraw %}