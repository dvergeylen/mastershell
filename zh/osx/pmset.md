---
layout: default
title: "pmset"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pmset">
  <a href="/zh/osx/pmset.html">pmset</a> <a href="#pmset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 配置 macOS 电源管理设置，就像在系统首选项 > 节能程序中一样.
> 修改设置的命令必须以 `sudo` 开头.

#### 显示当前电源管理设置:
```shell
pmset -g
```
#### 显示当前电源和电池电量:
```shell
pmset -g batt
```
#### 当充电器通电时，将显示器设置为从不休眠:
```shell
sudo pmset -c displaysleep 0
```
#### 使用电池电源 15 分钟后将显示器设置为休眠:
```shell
sudo pmset -b displaysleep 15
```
#### 安排计算机在每个工作日上午 9 点自动唤醒:
```shell
sudo pmset repeat wake MTWRF 09:00:00
```
#### 还原为系统默认值:
```shell
sudo pmset -a displaysleep 10 disksleep 10 sleep 30 womp 1
```
{% endraw %}