---
layout: default
title: "vsce"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="vsce">
  <a href="/en/common/vsce.html">vsce</a> <a href="#vsce"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extension manager for Visual Studio Code.
> More information: <https://github.com/microsoft/vscode-vsce>.

#### List all the extensions created by a publisher:
```shell
vsce list {{publisher}}
```
#### Publish an extension as major, minor or patch version:
```shell
vsce publish {{major|minor|patch}}
```
#### Unpublish an extension:
```shell
vsce unpublish {{extension_id}}
```
#### Package the current working directory as a `.vsix` file:
```shell
vsce package
```
#### Show the metadata associated with an extension:
```shell
vsce show {{extension_id}}
```
{% endraw %}