---
layout: default
title: "debuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="debuild">
  <a href="/zh/linux/debuild.html">debuild</a> <a href="#debuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从源代码构建 `Debian` 软件包的工具。
> 更多信息：<https://manpages.debian.org/debuild>.

#### 在当前目录中生成软件包：
```shell
debuild
```
#### 仅构建二进制包：
```shell
debuild -b
```
#### 生成软件包后，不运行 `lintian` （检查常见打包错误）：
```shell
debuild --no-lintian
```
{% endraw %}