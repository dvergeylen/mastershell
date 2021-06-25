---
layout: default
title: "phing"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phing">
  <a href="/en/common/phing.html">phing</a> <a href="#phing"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A PHP build tool based on Apache Ant.
> More information: <https://www.phing.info>.

#### Perform the default task in the `build.xml` file:
```shell
phing
```
#### Initialise a new build file:
```shell
phing -i {{path/to/build.xml}}
```
#### Perform a specific task:
```shell
phing {{task_name}}
```
#### Specify a custom build file path:
```shell
phing -f {{path/to/build.xml}} {{task_name}}
```
#### Specify a log file to output to:
```shell
phing -b {{path/to/log_file}} {{task_name}}
```
#### Specify custom properties to use in the build:
```shell
phing -D{{property}}={{value}} {{task_name}}
```
#### Specify a custom listener class:
```shell
phing -listener {{class_name}} {{task_name}}
```
#### Build using verbose output:
```shell
phing -verbose {{task_name}}
```
{% endraw %}