---
layout: default
title: "ansiweather"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansiweather">
  <a href="/zh/common/ansiweather.html">ansiweather</a> <a href="#ansiweather"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个 shell 脚本，用于在终端中显示当前的天气状况.

#### 使用公制单位显示 Rzeszow, Poland 接下来 5 天的天气预报:
```shell
ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}
```
#### 显示带符号和日光数据信息的天气预报:
```shell
ansiweather -s {{true}} -d {{true}}
```
#### 显示带风力等级和湿度信息的天气预报:
```shell
ansiweather -w {{true}} -h {{true}}
```
{% endraw %}