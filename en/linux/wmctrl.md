---
layout: default
title: "wmctrl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wmctrl">
  <a href="/en/linux/wmctrl.html">wmctrl</a> <a href="#wmctrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for X Window Manager.

#### List all windows, managed by the window manager:
```shell
wmctrl -l
```
#### Switch to the first window whose (partial) title matches:
```shell
wmctrl -a {{window_title}}
```
#### Move a window to the current workspace, raise it and give it focus:
```shell
wmctrl -R {{window_title}}
```
#### Switch to a workspace:
```shell
wmctrl -s {{workspace_number}}
```
#### Select a window and toggle fullscreen:
```shell
wmctrl -r {{window_title}} -b toggle,fullscreen
```
#### Select a window a move it to a workspace:
```shell
wmctrl -r {{window_title}} -t {{workspace_number}}
```
{% endraw %}