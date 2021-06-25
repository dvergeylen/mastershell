---
layout: default
title: "whereis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="whereis">
  <a href="/zh/osx/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 找到命令的二进制，源文件和手册文件.

#### 找到 `ssh` 命令的二进制、源文件和手册页:
```shell
whereis {{ssh}}
```
#### 查找 `ls` 命令的二进制和手册页:
```shell
whereis -bm {{ls}}
```
#### 找到 `gc` 的源文件和 `git` 的手册页:
```shell
whereis -s {{gcc}} -m {{git}}
```
#### 仅在 /usr/bin/ 目录中查找 `gcc` 的二进制文件:
```shell
whereis -b -B {{/usr/bin/}} -f {{gcc}}
```
{% endraw %}