---
layout: default
title: "swift"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="swift">
  <a href="/en/common/swift.html">swift</a> <a href="#swift"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, run and build Swift projects.
> More information: <https://swift.org>.

#### Invoke the interactive interpreter (REPL):
```shell
swift
```
#### Execute a program:
```shell
swift {{file.swift}}
```
#### Start a new project with the package manager:
```shell
swift package init
```
#### Generate an Xcode project file:
```shell
swift package generate-xcodeproj
```
#### Update dependencies:
```shell
swift package update
```
#### Compile project for release:
```shell
swift build -c release
```
{% endraw %}