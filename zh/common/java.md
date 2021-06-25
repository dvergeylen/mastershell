---
layout: default
title: "java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="java">
  <a href="/zh/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 程序启动器.
> 更多信息: <https://java.com>.

#### 通过提供类名称运行一个含有 main 函数的 java .class 程序:
```shell
java {{类名称}}
```
#### 运行一个 .jar 程序:
```shell
java -jar {{文件名.jar}}
```
#### 运行一个 .jar 程序并且在端口5005等待调试器:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{文件名.jar}}
```
#### 显示 JDK, JRE 和 HotSpot 的版本:
```shell
java -version
```
#### 显示详细的帮助:
```shell
java -help
```
{% endraw %}