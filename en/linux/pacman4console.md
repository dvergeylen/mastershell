---
layout: default
title: "pacman4console"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman4console">
  <a href="/en/linux/pacman4console.html">pacman4console</a> <a href="#pacman4console"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based console game inspired by the original Pacman.
> More information: <https://github.com/YoctoForBeaglebone/pacman4console>.

#### Start a game at Level 1:
```shell
pacman4console
```
#### Start a game on a certain level (there are nine official levels):
```shell
pacman4console --level={{level_number}}
```
#### Start the pacman4console level editor, saving to a specified text file:
```shell
pacman4consoleedit {{path/to/level_file}}
```
#### Play a custom level:
```shell
pacman4console --level={{path/to/level_file}}
```
{% endraw %}