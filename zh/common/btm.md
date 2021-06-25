---
layout: default
title: "btm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="btm">
  <a href="/zh/common/btm.html">btm</a> <a href="#btm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令行`top`的替代品.
> 比`top更轻便，支持跨平台、图表更丰富`.
> 更多信息: <https://github.com/ClementTsang/bottom>.

#### 展示默认布局 (cpu, 内存, 温度, 磁盘, 网络和 进程):
```shell
btm
```
#### 开启基础模式,关闭图表和高亮(接近于 `top`):
```shell
btm --basic
```
#### 将图表中的小点换成大点:
```shell
btm --dot_marker
```
#### 展示电池充电和健康状态:
```shell
btm --battery
```
#### 设置图表刷新间隔和留存数据的时长:
```shell
btm --rate 250 --default_time_value 30000
```
{% endraw %}