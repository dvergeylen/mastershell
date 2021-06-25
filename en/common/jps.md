---
layout: default
title: "jps"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jps">
  <a href="/en/common/jps.html">jps</a> <a href="#jps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show JVM Process Status of current user.
> More information: <https://docs.oracle.com/en/java/javase/11/tools/jps.html>.

#### List all JVM processes:
```shell
jps
```
#### List all JVM processes with only PID:
```shell
jps -q
```
#### Display the arguments passed to the processes:
```shell
jps -m
```
#### Display the full package name of all processes:
```shell
jps -l
```
#### Display the arguments passed to the JVM:
```shell
jps -v
```
{% endraw %}