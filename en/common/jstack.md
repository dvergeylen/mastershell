---
layout: default
title: "jstack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="jstack">
  <a href="/en/common/jstack.html">jstack</a> <a href="#jstack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Stack Trace Tool.

#### Print java stack traces for all threads in a java process:
```shell
jstack {{java_pid}}
```
#### Print mixed mode (java/c++) stack traces for all threads in a java process:
```shell
jstack -m {{java_pid}}
```
#### Print stack traces from java core dump:
```shell
jstack {{/usr/bin/java}} {{file.core}}
```
{% endraw %}