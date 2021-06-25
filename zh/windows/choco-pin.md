---
layout: default
title: "choco pin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-pin">
  <a href="/zh/windows/choco-pin.html">choco pin</a> <a href="#choco-pin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 将一个包固定到指定的版本.
> 被固定版本的包会在更新时自动忽略.

#### 显示被固定的包以及他们对应的版本号:
```shell
choco pin list
```
#### 将一个包固定至当前版本:
```shell
choco pin add --name {{包名}}
```
#### 将一个包固定直指定的版本:
```shell
choco pin add --name {{包名}} --version {{版本号}}
```
#### 移除指定包的固定状态:
```shell
choco pin remove --name {{包名}}
```
{% endraw %}