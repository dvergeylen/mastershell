---
layout: default
title: "carthage"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="carthage">
  <a href="/en/osx/carthage.html">carthage</a> <a href="#carthage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A dependency management tool for Cocoa applications.

#### Download the latest version of all dependencies mentioned in Cartfile, and build them:
```shell
carthage update
```
#### Update dependencies, but only build for iOS:
```shell
carthage update --platform ios
```
#### Update dependencies, but don't build any of them:
```shell
carthage update --no-build
```
#### Download and rebuild the current version of dependencies (without updating them):
```shell
carthage bootstrap
```
#### Rebuild a specific dependency:
```shell
carthage build {{dependency}}
```
{% endraw %}