---
layout: default
title: "yay"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yay">
  <a href="/zh/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt: 一个用于 Arch Linux 的工具，用于从 Arch User Repository 中构建和安装软件包。
> 另见 `pacman`。
> 更多信息: <https://github.com/Jguer/yay>.

#### 从仓库和 AUR 中交互式搜索和安装软件包：
```shell
yay {{软件包|搜索词}}
```
#### 同步并更新所有来自仓库和 AUR 的软件包：
```shell
yay
```
#### 只同步和更新 AUR 软件包：
```shell
yay -Sua
```
#### 从仓库和 AUR 中安装一个新的软件包。
```shell
yay -S {{软件包}}
```
#### 从仓库和 AUR 中搜索软件包数据库中的关键词：
```shell
yay -Ss {{关键词}}
```
#### 显示已安装软件包和系统健康状况的统计数据：
```shell
yay -Ps
```
{% endraw %}