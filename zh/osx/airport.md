---
layout: default
title: "airport"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="airport">
  <a href="/zh/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 无线网络配置工具.

#### 显示当前的无线状态信息:
```shell
airport -I
```
#### 在通道 1 上监察（嗅探）无线流量:
```shell
airport sniff {{1}}
```
#### 扫描可用的无线网络:
```shell
airport -s
```
#### 与当前的 Airport 网络脱离连接:
```shell
sudo airport -z
```
{% endraw %}