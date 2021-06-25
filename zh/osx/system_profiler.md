---
layout: default
title: "system_profiler"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="system_profiler">
  <a href="/zh/osx/system_profiler.html">system_profiler</a> <a href="#system_profiler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 报告系统硬件和软件配置.

#### 显示可由 System Profiler.app 打开的完整系统资源报告:
```shell
system_profiler -xml > MyReport.spx
```
#### 显示硬件概述（型号、CPU、内存、串行等）:
```shell
system_profiler SPHardwareDataType
```
#### 打印系统序列号:
```shell
system_profiler SPHardwareDataType|grep "Serial Number (system)" |awk '{print $4}'
```
{% endraw %}