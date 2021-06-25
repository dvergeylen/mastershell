---
layout: default
title: "choco outdated"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="choco-outdated">
  <a href="/zh/windows/choco-outdated.html">choco outdated</a> <a href="#choco-outdated"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Chocolatey 检查过时的包.

#### 用表格的形式列出过时的包:
```shell
choco outdated
```
#### 忽略输出中的固定包:
```shell
choco outdated --ignore-pinned
```
#### 从自定义的源处检查过时的包:
```shell
choco outdated --source {{源 URL|别名}}
```
#### 提供一个用户名和密码来进行验证:
```shell
choco outdated --user {{用户名}} --password {{密码}}
```
{% endraw %}