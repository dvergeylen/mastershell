---
layout: default
title: "scoop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scoop">
  <a href="/zh/windows/scoop.html">scoop</a> <a href="#scoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Windows 的命令行安装程序.

#### 安装一个包:
```shell
scoop install {{包名}}
```
#### 删除一个包:
```shell
scoop uninstall {{包名}}
```
#### 更新所有已安装的包:
```shell
scoop update *
```
#### 列出所有已安装的包:
```shell
scoop list
```
#### 显示一个包的信息:
```shell
scoop info {{包名}}
```
#### 搜索一个包:
```shell
scoop search {{包名}}
```
#### 列出所有已知的桶 (“桶”代表程序的仓库）:
```shell
scoop bucket known
```
#### 通过别名或 Git 存储库 URL 添加存储桶:
```shell
scoop bucket add {{bucket}}
```
{% endraw %}