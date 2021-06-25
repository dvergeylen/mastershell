---
layout: default
title: "units"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="units">
  <a href="/zh/common/units.html">units</a> <a href="#units"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 提供两个度量单位之间的转换.
> 更多信息： <https://www.gnu.org/software/units/>.

#### 以交互模式运行:
```shell
units
```
#### 显示两个简单单位之间的转换:
```shell
units {{quarts（夸脱）}} {{tablespoons（大汤匙）}}
```
#### 单位与数量之间的转换:
```shell
units "{{15 pounds（磅）}}" {{kilograms（公斤）}}
```
#### 显示两个复合单位之间的转换:
```shell
units "{{meters（米） / second（秒）}}" "{{inches（英尺） / hour（小时）}}"
```
#### 显示具有不同维度的单位之间的转换:
```shell
units "{{acres（英亩）}}" "{{ft（英尺）^2（平方）}}"
```
#### 显示字节乘数的转换:
```shell
units "{{15 megabytes（兆字节）}}" {{bytes（字节）}}
```
{% endraw %}