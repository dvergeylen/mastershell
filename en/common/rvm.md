---
layout: default
title: "rvm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rvm">
  <a href="/en/common/rvm.html">rvm</a> <a href="#rvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for easily installing, managing, and working with multiple ruby environments.
> More information: <https://rvm.io>.

#### Install one or more space-separated versions of Ruby:
```shell
rvm install {{version(s)}}
```
#### Display a list of installed versions:
```shell
rvm list
```
#### Use a specific version of Ruby:
```shell
rvm use {{version}}
```
#### Set the default Ruby version:
```shell
rvm --default use {{version}}
```
#### Upgrade a version of Ruby to a new version:
```shell
rvm upgrade {{current_version}} {{new_version}}
```
#### Uninstall a version of Ruby and keep its sources:
```shell
rvm uninstall {{version}}
```
#### Remove a version of Ruby and its sources:
```shell
rvm remove {{version}}
```
#### Show specific dependencies for your OS:
```shell
rvm requirements
```
{% endraw %}