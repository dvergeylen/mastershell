---
layout: default
title: "mvn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mvn">
  <a href="/zh/common/mvn.html">mvn</a> <a href="#mvn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Maven.
> 用于构建和管理基于 Java 的项目的工具。
> 更多信息见：<https://maven.apache.org>.

#### 编译项目：
```shell
mvn compile
```
#### 将编译后的代码打包成可分发格式，比如 `jar`：
```shell
mvn package
```
#### 编译和打包，跳过单元测试：
```shell
mvn package -Dmaven.test.skip=true
```
#### 在本地 maven 存储库中安装构建的包（这也会调用 compile 和 package 命令）：
```shell
mvn install
```
#### 从目标目录中删除构建工件，通常用来清理之前的编译结果：
```shell
mvn clean
```
#### 执行清理操作，然后进行编译打包：
```shell
mvn clean package
```
#### 执行清理操作并使用给定的构建配置打包代码，比如 `profileId` 如果有dev、test、pro，可以指定其中一个 `profileId` 用来选择具体执行环境：
```shell
mvn clean -P{{profileId}} package
```
#### 使用 main 方法运行一个类：
```shell
mvn exec:java -Dexec.mainClass="{{com.example.Main}}" -Dexec.args="{{参数1 参数2}}"
```
{% endraw %}