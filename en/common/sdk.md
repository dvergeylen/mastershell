---
layout: default
title: "sdk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sdk">
  <a href="/en/common/sdk.html">sdk</a> <a href="#sdk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing parallel versions of multiple Software Development Kits.
> Supports Java, Groovy, Scala, Kotlin, Gradle, Maven, Vert.x and many others.
> More information: <https://sdkman.io/usage>.

#### Install a specific version of Gradle:
```shell
sdk install {{gradle}} {{gradle_version}}
```
#### Switch to a specific version of Gradle:
```shell
sdk use {{gradle}} {{gradle_version}}
```
#### Check current Gradle version:
```shell
sdk current {{gradle}}
```
#### List all Software Development Kits available to install:
```shell
sdk list
```
#### Update Gradle to the latest version:
```shell
sdk upgrade {{gradle}}
```
#### Uninstall a particular version of Gradle:
```shell
sdk rm {{gradle}} {{gradle_version}}
```
{% endraw %}