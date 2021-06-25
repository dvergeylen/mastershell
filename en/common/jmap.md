---
layout: default
title: "jmap"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jmap">
  <a href="/en/common/jmap.html">jmap</a> <a href="#jmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Memory Map Tool.

#### Print shared object mappings for a java process (output like pmap):
```shell
jmap {{java_pid}}
```
#### Print heap summary information:
```shell
jmap -heap {{filename.jar}} {{java_pid}}
```
#### Print histogram of heap usage by type:
```shell
jmap -histo {{java_pid}}
```
#### Dump contents of the heap into a binary file for analysis with jhat:
```shell
jmap -dump:format=b,file={{filename}} {{java_pid}}
```
{% endraw %}