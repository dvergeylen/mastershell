---
layout: default
title: "javac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="javac">
  <a href="/zh/common/javac.html">javac</a> <a href="#javac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 程序编译器.

#### 编译一个 `.java` 文件:
```shell
javac {{文件名.java}}
```
#### 编译多个 `.java` 文件:
```shell
javac {{文件名1.java}} {{文件名2.java}} {{文件名3.java}}
```
#### 编译当前目录内所有 `.java` 文件:
```shell
javac {{*.java}}
```
#### 编译一个 `.java` 文件并将生成的 class 字节码文件放入一个指定目录:
```shell
javac -d {{输出目录}} {{文件名.java}}
```
{% endraw %}