---
layout: default
title: "pod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pod">
  <a href="/en/osx/pod.html">pod</a> <a href="#pod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dependency manager for Swift and Objective-C Cocoa projects.

#### Create a Podfile for the current project with the default contents:
```shell
pod init
```
#### Download and install all pods defined in the Podfile (that haven't been installed before):
```shell
pod install
```
#### List all available pods:
```shell
pod list
```
#### Show the outdated pods (of those currently installed):
```shell
pod outdated
```
#### Update all currently installed pods to their newest version:
```shell
pod update
```
#### Update a specific (previously installed) pod to its newest version:
```shell
pod update {{pod_name}}
```
#### Remove CocoaPods from a Xcode project:
```shell
pod deintegrate {{xcode_project}}
```
{% endraw %}