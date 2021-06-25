---
layout: default
title: "xctool"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xctool">
  <a href="/en/osx/xctool.html">xctool</a> <a href="#xctool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for building Xcode projects.
> More information: <https://github.com/facebook/xctool>.

#### Build a single project without any workspace:
```shell
xctool -project {{YourProject.xcodeproj}} -scheme {{YourScheme}} build
```
#### Build a project that is part of a workspace:
```shell
xctool -workspace {{YourWorkspace.xcworkspace}} -scheme {{YourScheme}} build
```
#### Clean, build and execute all the tests:
```shell
xctool -workspace {{YourWorkspace.xcworkspace}} -scheme {{YourScheme}} clean build test
```
{% endraw %}