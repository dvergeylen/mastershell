---
layout: default
title: "pacman"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pacman">
  <a href="/zh/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux 的软件包管理器工具。
> 更多信息: <https://man.archlinux.org/man/pacman.8>.

#### 同步并更新所有软件包：
```shell
pacman -Syu
```
#### 安装一个新的软件包：
```shell
pacman -S {{软件包}}
```
#### 删除一个软件包及其依赖：
```shell
pacman -Rs {{软件包}}
```
#### 在软件包数据库中搜索正则表达式或关键字：
```shell
pacman -Ss "{{软件包}}"
```
#### 列出已安装的软件包和版本：
```shell
pacman -Q
```
#### 仅列出明确安装的软件包和版本：
```shell
pacman -Qe
```
#### 查找哪个包拥有某个文件：
```shell
pacman -Qo {{文件名}}
```
#### 清空软件包缓存以释放空间：
```shell
pacman -Scc
```
{% endraw %}