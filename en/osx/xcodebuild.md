---
layout: default
title: "xcodebuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xcodebuild">
  <a href="/en/osx/xcodebuild.html">xcodebuild</a> <a href="#xcodebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build Xcode projects.

#### Build workspace:
```shell
xcodebuild -workspace {{workspace_name.workspace}} -scheme {{scheme_name}} -configuration {{configuration_name}} clean build SYMROOT={{SYMROOT_path}}
```
#### Build project:
```shell
xcodebuild -target {{target_name}} -configuration {{configuration_name}} clean build SYMROOT={{SYMROOT_path}}
```
#### Show SDKs:
```shell
xcodebuild -showsdks
```
{% endraw %}