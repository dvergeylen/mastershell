---
layout: default
title: "acpi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="acpi">
  <a href="/zh/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示电池状态或热量信息。
> 更多信息：<https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### 显示电池信息：
```shell
acpi
```
#### 显示热量（温度）信息：
```shell
acpi -t
```
#### 显示冷却设备信息：
```shell
acpi -c
```
#### 用华氏度单位显示热量（温度）信息：
```shell
acpi -tf
```
#### 显示所有信息：
```shell
acpi -V
```
#### 从 `/proc` 而非 `/sys` 中提取信息：
```shell
acpi -p
```
{% endraw %}