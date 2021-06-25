---
layout: default
title: "banner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="banner">
  <a href="/zh/common/banner.html">banner</a> <a href="#banner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将给定参数输出为大型 ASCII 文字.
> 更多信息： <https://man.archlinux.org/man/banner.1>.

#### 将文字信息打印为大横幅（引号是可选的）:
```shell
banner "{{Hello World}}"
```
#### 将文字信息打印为横幅，宽度为 50 个字:
```shell
banner -w {{50}} "{{Hello World}}"
```
#### 从 stdin 中读取文本:
```shell
banner
```
{% endraw %}