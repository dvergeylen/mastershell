---
layout: default
title: "bower"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bower">
  <a href="/en/common/bower.html">bower</a> <a href="#bower"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A package manager optimized for front-end web development.
> A package can be a GitHub user/repo shorthand, a Git endpoint, a URL or a registered package.
> More information: <https://bower.io/>.

#### Install a project's dependencies, listed in its bower.json:
```shell
bower install
```
#### Install one or more packages to the bower_components directory:
```shell
bower install {{package}} {{package}}
```
#### Uninstall packages locally from the bower_components directory:
```shell
bower uninstall {{package}} {{package}}
```
#### List local packages and possible updates:
```shell
bower list
```
#### Display help information about a bower command:
```shell
bower help {{command}}
```
#### Create a `bower.json` file for your package:
```shell
bower init
```
#### Install a specific dependency version, and add it to `bower.json`:
```shell
bower install {{local_name}}={{package}}#{{version}} --save
```
{% endraw %}