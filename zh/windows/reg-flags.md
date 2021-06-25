---
layout: default
title: "reg flags"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-flags">
  <a href="/zh/windows/reg-flags.html">reg flags</a> <a href="#reg-flags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置注册表键的标志.

#### 显示当前指定键的标志:
```shell
reg flags {{键名}} query
```
#### 显示帮助和可用的标志类型:
```shell
reg flags /?
```
#### 为特定键设置指定以空格分隔的标志，并取消设置未提及的标志:
```shell
reg flags {{键名}} set {{标志 1 标志 2 ..}}
```
#### 为指定的键和其子键设置标志:
```shell
reg flags {{键名}} set {{标志}} /s
```
{% endraw %}