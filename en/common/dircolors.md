---
layout: default
title: "dircolors"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dircolors">
  <a href="/en/common/dircolors.html">dircolors</a> <a href="#dircolors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output commands to set the LS_COLOR environment variable and style `ls`, `dir`, etc.
> More information: <https://www.gnu.org/software/coreutils/dircolors>.

#### Output commands to set LS_COLOR using default colors:
```shell
dircolors
```
#### Output commands to set LS_COLOR using colors from a file:
```shell
dircolors {{file}}
```
#### Output commands for Bourne shell:
```shell
dircolors --bourne-shell
```
#### Output commands for C shell:
```shell
dircolors --c-shell
```
#### View the default colors for file types and extensions:
```shell
dircolors --print-data
```
{% endraw %}