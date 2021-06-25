---
layout: default
title: "sbt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sbt">
  <a href="/en/common/sbt.html">sbt</a> <a href="#sbt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build tool for Scala and Java projects.
> More information: <https://www.scala-sbt.org/1.0/docs/>.

#### Start the SBT interactive shell (REPL):
```shell
sbt
```
#### Create a new Scala project from an existing Giter8 template hosted on GitHub:
```shell
sbt new {{scala/hello-world.g8}}
```
#### Use the specified version of sbt:
```shell
sbt -sbt-version {{version}}
```
#### Use a specific jar file as the sbt launcher:
```shell
sbt -sbt-jar {{path}}
```
#### List all sbt options:
```shell
sbt -h
```
{% endraw %}