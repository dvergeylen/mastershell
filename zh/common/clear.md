---
layout: default
title: "clear"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="clear">
  <a href="/zh/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 清空终端的屏幕.
> 更多信息： <https://manned.org/clear>.

#### 清空屏幕（相当于在 Bash shell 中按 Control-L 键）:
```shell
clear
```
#### 清空屏幕但保留终端的回滚缓冲区:
```shell
clear -x
```
#### 指明要清空的终端类型（默认为环境变量 `TERM` 的值）:
```shell
clear -T {{type_of_terminal}}
```
#### 显示 `clear` 使用的 `ncurses` 版本:
```shell
clear -V
```
{% endraw %}