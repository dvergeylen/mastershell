---
layout: default
title: "tput"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="tput">
  <a href="/en/common/tput.html">tput</a> <a href="#tput"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View and modify terminal settings and capabilities.

#### Move the cursor to a screen location:
```shell
tput cup {{y_coordinate}} {{x_coordinate}}
```
#### Set foreground (af) or background (ab) color:
```shell
tput {{setaf|setab}} {{ansi_color_code}}
```
#### Show number of columns, lines, or colors:
```shell
tput {{cols|lines|colors}}
```
#### Ring the terminal bell:
```shell
tput bel
```
#### Reset all terminal attributes:
```shell
tput sgr0
```
#### Enable / Disable word wrap:
```shell
tput {{smam|rmam}}
```
{% endraw %}