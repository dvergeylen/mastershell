---
layout: default
title: "nodemon"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nodemon">
  <a href="/en/common/nodemon.html">nodemon</a> <a href="#nodemon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Watch files and automatically restart a node application when changes are detected.
> More information: <https://nodemon.io>.

#### Execute the specified file and watch a specific file for changes:
```shell
nodemon --inspect {{path/to/file.js}}
```
#### Manually restart nodemon (note nodemon must already be active for this to work):
```shell
rs
```
#### Ignore specific files:
```shell
nodemon --ignore {{path/to/file_or_directory}}
```
#### Pass arguments to the node application:
```shell
nodemon {{path/to/file.js}} {{arguments}}
```
#### Run non-node scripts:
```shell
nodemon --exec "{{python --verbose}}" {{path/to/file.py}}
```
{% endraw %}