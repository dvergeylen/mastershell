---
layout: default
title: "slop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="slop">
  <a href="/en/linux/slop.html">slop</a> <a href="#slop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get a selection of the screen.
> More information: <https://github.com/naelstrof/slop>.

#### Wait for the user to make a selection and output its geometry to standard output:
```shell
slop
```
#### Double click, rather than click and drag, to draw a selection:
```shell
slop -D
```
#### Highlight the selection rather than outlining it:
```shell
slop -l
```
#### Specify the output format:
```shell
slop -f {{format_string}}
```
#### Specify the selection rectangle's color:
```shell
slop -c {{red}},{{green}},{{blue}},{{alpha}}
```
{% endraw %}