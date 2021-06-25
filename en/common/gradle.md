---
layout: default
title: "gradle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gradle">
  <a href="/en/common/gradle.html">gradle</a> <a href="#gradle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gradle is an open source build automation system.
> More information: <https://gradle.org>.

#### Compile a package:
```shell
gradle build
```
#### Exclude test task:
```shell
gradle build -x {{test}}
```
#### Run in offline mode to prevent gradle from accessing the network during builds:
```shell
gradle build --offline
```
#### Clear the build directory:
```shell
gradle clean
```
#### Compile and Release package:
```shell
gradle assembleRelease
```
#### List the main tasks:
```shell
gradle tasks
```
#### List all the tasks:
```shell
gradle tasks --all
```
{% endraw %}