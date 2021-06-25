---
layout: default
title: "n"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="n">
  <a href="/en/osx/n.html">n</a> <a href="#n"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manage multiple node versions.

#### Install a given version of node. If the version is already installed, it will be activated:
```shell
n {{version}}
```
#### Display installed versions and interactively activate one of them:
```shell
n
```
#### Remove a version:
```shell
n rm {{version}}
```
#### Execute a file with a given version:
```shell
n use {{version}} {{file.js}}
```
#### Output binary path for a version:
```shell
n bin {{version}}
```
{% endraw %}