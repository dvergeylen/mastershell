---
layout: default
title: "mvn"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="mvn">
  <a href="/en/common/mvn.html">mvn</a> <a href="#mvn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Maven.
> Tool for building and managing Java-based projects.
> More information: <https://maven.apache.org>.

#### Compile a project:
```shell
mvn compile
```
#### Compile and package the compiled code in its distributable format, such as a `jar`:
```shell
mvn package
```
#### Compile and package, skipping unit tests:
```shell
mvn package -Dmaven.test.skip=true
```
#### Install the built package in local maven repository. (This will invoke the compile and package commands too):
```shell
mvn install
```
#### Delete build artifacts from the target directory:
```shell
mvn clean
```
#### Do a clean and then invoke the package phase:
```shell
mvn clean package
```
#### Clean and then package the code with a given build profile:
```shell
mvn clean -P{{profile}} package
```
#### Run a class with a main method:
```shell
mvn exec:java -Dexec.mainClass="{{com.example.Main}}" -Dexec.args="{{arg1 arg2}}"
```
{% endraw %}