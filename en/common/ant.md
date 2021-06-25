---
layout: default
title: "ant"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ant">
  <a href="/en/common/ant.html">ant</a> <a href="#ant"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Ant.
> Tool for building and managing Java-based projects.
> More information: <https://ant.apache.org>.

#### Build a project with default build file `build.xml`:
```shell
ant
```
#### Build a project using build file other than `build.xml`:
```shell
ant -f {{buildfile.xml}}
```
#### Print information on possible targets for this project:
```shell
ant -p
```
#### Print debugging information:
```shell
ant -d
```
#### Execute all targets that do not depend on fail target(s):
```shell
ant -k
```
{% endraw %}