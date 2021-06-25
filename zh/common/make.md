---
layout: default
title: "make"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="make">
  <a href="/zh/common/make.html">make</a> <a href="#make"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Makefile 文件描述目标的任务运行器。
> 通常用于控制源代码中可执行文件的编译。
> 更多信息见：<https://www.gnu.org/software/make/manual/make.html>.

#### 调用 Makefile 中指定的第一个目标（通常命名为 "all"）：
```shell
make
```
#### 调用指定目标：
```shell
make {{目标}}
```
#### 调用一个指定的目标，一次并行执行4个作业：
```shell
make -j{{4}} {{目标}}
```
#### 使用指定的 Makefile 文件：
```shell
make --file {{文件}}
```
#### 从另一个目录执行 make ：
```shell
make --directory {{文件夹}}
```
#### 即使源文件未更改，也强制执行目标：
```shell
make --always-make {{目标}}
```
#### 覆盖在 Makefile 中定义的环境变量：
```shell
make --environment-overrides {{目标}}
```
{% endraw %}