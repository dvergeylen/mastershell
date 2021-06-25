---
layout: default
title: "scala"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scala">
  <a href="/en/common/scala.html">scala</a> <a href="#scala"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scala application launcher and interactive interpreter.
> More information: <https://scala-lang.org>.

#### Start a Scala interactive shell (REPL):
```shell
scala
```
#### Start the interpreter with a dependency in the classpath:
```shell
scala -classpath {{filename.jar}} {{command}}
```
#### Execute a Scala script:
```shell
scala {{script.scala}}
```
#### Execute a `.jar` program:
```shell
scala {{filename.jar}}
```
#### Execute a single Scala command in the command-line:
```shell
scala -e {{command}}
```
{% endraw %}