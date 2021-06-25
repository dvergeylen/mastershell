---
layout: default
title: "apt-mark"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="apt-mark">
  <a href="/zh/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 修改已安装软件包状态的工具
> 更多信息： <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### 将一个软件包标记为自动安装:
```shell
sudo apt-mark auto {{软件包名}}
```
#### 将一个软件包保持在当前版本，防止对其更新:
```shell
sudo apt-mark hold {{软件包名}}
```
#### 允许对一个软件包更新:
```shell
sudo apt-mark unhold {{软件包名}}
```
#### 列出手动安装的软件包:
```shell
apt-mark showmanual
```
#### 列出保持当前版本而不更新的软件包:
```shell
apt-mark showhold
```
{% endraw %}