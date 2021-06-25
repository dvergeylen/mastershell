---
layout: default
title: "java"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="java">
  <a href="/en/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Application Launcher.
> More information: <https://java.com>.

#### Execute a java `.class` file that contains a main method by using just the class name:
```shell
java {{classname}}
```
#### Execute a `.jar` program:
```shell
java -jar {{filename.jar}}
```
#### Execute a `.jar` program with debug waiting to connect on port 5005:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{filename.jar}}
```
#### Display JDK, JRE and HotSpot versions:
```shell
java -version
```
#### Display usage information for the java command:
```shell
java -help
```
{% endraw %}