---
layout: default
title: "scrot"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scrot">
  <a href="/en/linux/scrot.html">scrot</a> <a href="#scrot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screen capture utility.
> More information: <https://github.com/resurrecting-open-source-projects/scrot>.

#### Capture a screenshot and save it to the current directory with the current date as the filename:
```shell
scrot
```
#### Capture a screenshot and save it as `capture.png`:
```shell
scrot {{capture.png}}
```
#### Capture a screenshot interactively:
```shell
scrot --select
```
#### Capture a screenshot from the currently focused window:
```shell
scrot --focused
```
#### Display a countdown of 10 seconds before taking a screenshot:
```shell
scrot --count --delay {{10}}
```
{% endraw %}