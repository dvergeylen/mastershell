---
layout: default
title: "phive"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phive">
  <a href="/en/common/phive.html">phive</a> <a href="#phive"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Phar Installation and Verification Environment for secure PHP application deployment.
> More information: <https://phar.io>.

#### Display a list of available aliased Phars:
```shell
phive list
```
#### Install a specified Phar to the local directory:
```shell
phive install {{alias|url}}
```
#### Install a specified Phar globally:
```shell
phive install {{alias|url}} --global
```
#### Install a specified Phar to a target directory:
```shell
phive install {{alias|url}} --target {{path/to/directory}}
```
#### Update all Phar files to the latest version:
```shell
phive update
```
#### Remove a specified Phar file:
```shell
phive remove {{alias|url}}
```
#### Remove unused Phar files:
```shell
phive purge
```
#### List all available commands:
```shell
phive help
```
{% endraw %}