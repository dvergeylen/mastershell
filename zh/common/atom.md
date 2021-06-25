---
layout: default
title: "atom"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="atom">
  <a href="/zh/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个跨平台的，可插拔的文本编辑器.
> 由 `apm` 管理插件.
> 更多信息：<https://atom.io/>.

#### 打开文件或目录:
```shell
atom {{path/to/file_or_directory}}
```
#### 在新窗口中打开文件或目录:
```shell
atom -n {{path/to/file_or_directory}}
```
#### 在已有窗口中打开文件或目录:
```shell
atom --add {{path/to/file_or_directory}}
```
#### 以安全模式启动 Atom （不加载额外插件）:
```shell
atom --safe
```
#### 在终端前台运行 Atom:
```shell
atom --foreground
```
{% endraw %}