---
layout: default
title: "cp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cp">
  <a href="/zh/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和文件夹。
> 更多信息：<https://www.gnu.org/software/coreutils/cp>.

#### 将文件复制到另一个位置：
```shell
cp {{某路径/源文件.ext}} {{某路径/目标文件.ext}}
```
#### 将文件复制到另一个文件夹，并保留原来的文件名：
```shell
cp {{某路径/源文件.ext}} {{某路径/目标文件夹}}
```
#### 以递归方式将文件夹内的内容复制到另一个位置（如果目标文件夹存在，则将此文件夹复制到目标文件夹中）：
```shell
cp -R {{某路径/源文件夹}} {{某路径/目标文件夹}}
```
#### 以详细模式递归复制目录（在复制文件时显示文件信息）：
```shell
cp -vR {{某路径/源文件夹}} {{某路径/目标文件夹}}
```
#### 以交互方式将文本文件复制到另一个位置（覆盖之前会提示用户）：
```shell
cp -i {{*.txt}} {{某路径/目标文件夹}}
```
#### 复制之前，请遵循符号链接：
```shell
cp -L {{符号文件}} {{某路径/目标文件夹}}
```
{% endraw %}