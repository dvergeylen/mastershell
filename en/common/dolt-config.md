---
layout: default
title: "dolt config"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dolt-config">
  <a href="/en/common/dolt-config.html">dolt config</a> <a href="#dolt-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and write local (per repository) and global (per user) Dolt configuration variables.
> More information: <https://docs.dolthub.com/interfaces/cli#dolt-config>.

#### List all local and global configuration options and their values:
```shell
dolt config --list
```
#### Display the value of a local or global configuration variable:
```shell
dolt config --get {{name}}
```
#### Modify the value of a local configuration variable, creating it if does not exist:
```shell
dolt config --add {{name}} {{value}}
```
#### Modify the value of a global configuration variable, creating it if does not exist:
```shell
dolt config --global --add {{name}} {{value}}
```
#### Delete a local configuration variable:
```shell
dolt config --unset {{name}}
```
#### Delete a global configuration variable:
```shell
dolt config --global --unset {{name}}
```
{% endraw %}