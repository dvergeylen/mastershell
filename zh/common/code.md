---
layout: default
title: "code"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="code">
  <a href="/zh/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> 更多信息: <https://github.com/microsoft/vscode>.

#### 打开 VS Code:
```shell
code
```
#### 在 VS Code 中打开当前目录:
```shell
code .
```
#### 在 VS Code 打开一个文件或目录:
```shell
code {{路径/文件或目录}}
```
#### 在当前打开的 VS Code 窗口中打开一个文件或目录:
```shell
code --reuse-window {{路径/文件或目录}}
```
#### 在 VS Code 中对比两个文件:
```shell
code -d {{文件1}} {{文件2}}
```
#### 用超级用户 (sudo) 权限打开 VS Code:
```shell
sudo code {{路径/文件或目录}} --user-data-dir
```
{% endraw %}