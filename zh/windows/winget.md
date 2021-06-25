---
layout: default
title: "winget"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="winget">
  <a href="/zh/windows/winget.html">winget</a> <a href="#winget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 软件包管理器命令行工具.
> 更多信息: <https://docs.microsoft.com/windows/package-manager/winget>.

#### 安装一个软件包:
```shell
winget install {{package}}
```
#### 显示关于一个软件包的信息:
```shell
winget show {{package}}
```
#### 查找一个软件包:
```shell
winget search {{package}}
```
{% endraw %}