---
layout: default
title: "yaourt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yaourt">
  <a href="/zh/linux/yaourt.html">yaourt</a> <a href="#yaourt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux 中用于从 Arch User Repository 中构建软件包的工具。

#### 同步并更新所有软件包（包括 AUR）：
```shell
yaourt -Syua
```
#### 安装一个新的软件包（包括 AUR）：
```shell
yaourt -S {{软件包}}
```
#### 移除一个软件包和它的依赖（包括 AUR 软件包）：
```shell
yaourt -Rs {{软件包}}
```
#### 在软件包数据库中搜索一个关键字（包括 AUR）：
```shell
yaourt -Ss {{软件包}}
```
#### 列出已安装的软件包、版本和仓库（AUR 软件包将被列在 'local' 仓库下):
```shell
yaourt -Q
```
{% endraw %}