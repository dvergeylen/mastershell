---
layout: default
title: "javac"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="javac">
  <a href="/en/common/javac.html">javac</a> <a href="#javac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java Application Compiler.

#### Compile a `.java` file:
```shell
javac {{file.java}}
```
#### Compile several `.java` files:
```shell
javac {{file1.java}} {{file2.java}} {{file3.java}}
```
#### Compile all `.java` files in current directory:
```shell
javac {{*.java}}
```
#### Compile a `.java` file and place the resulting class file in a specific directory:
```shell
javac -d {{path/to/some/directory}} {{file.java}}
```
{% endraw %}