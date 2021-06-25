---
layout: default
title: "ansiweather"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansiweather">
  <a href="/en/common/ansiweather.html">ansiweather</a> <a href="#ansiweather"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A shell script for displaying the current weather conditions in your terminal.
> More information: <https://github.com/fcambus/ansiweather>.

#### Display a forecast using metric units for the next five days for Rzeszow, Poland:
```shell
ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}
```
#### Display a forecast showing symbols and daylight data for your current location:
```shell
ansiweather -s {{true}} -d {{true}}
```
#### Display a forecast showing wind and humidity data for your current location:
```shell
ansiweather -w {{true}} -h {{true}}
```
{% endraw %}