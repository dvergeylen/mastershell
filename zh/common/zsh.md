---
layout: default
title: "zsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zsh">
  <a href="/zh/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell.
> 与 `bash` 和 `sh` 兼容的命令行解释器.
> 更多信息：<https://www.zsh.org>.

#### 启动交互式解释器:
```shell
zsh
```
#### 执行从参数传入的命令:
```shell
zsh -c {{command}}
```
#### 从文件执行命令 （脚本）:
```shell
zsh {{file}}
```
#### 从文件执行命令并将执行过的命令打印到终端:
```shell
zsh -x {{file}}
```
{% endraw %}