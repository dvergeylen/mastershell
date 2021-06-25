---
layout: default
title: "dmenu"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dmenu">
  <a href="/en/linux/dmenu.html">dmenu</a> <a href="#dmenu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dynamic menu.
> Creates a menu from a text input with each item on a new line.

#### Display a menu of the output of the `ls` command:
```shell
{{ls}} | dmenu
```
#### Display a menu with custom items separated by a new line (`\n`):
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu
```
#### Let the user choose between multiple items and save the selected one to a file:
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}
```
#### Launch dmenu on a specific monitor:
```shell
ls | dmenu -m {{1}}
```
#### Display dmenu at the bottom of the screen:
```shell
ls | dmenu -b
```
{% endraw %}