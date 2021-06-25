---
layout: default
title: "gibo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gibo">
  <a href="/en/common/gibo.html">gibo</a> <a href="#gibo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fetch gitignore boilerplates.
> More information: <https://github.com/simonwhitaker/gibo>.

#### List available boilerplates:
```shell
gibo list
```
#### Write a boilerplate to stdout:
```shell
gibo dump {{boilerplate}}
```
#### Write a boilerplate to .gitignore:
```shell
gibo dump {{boilerplate}} >>{{.gitignore}}
```
#### Search for boilerplates containing a given string:
```shell
gibo search {{string}}
```
#### Update available local boilerplates:
```shell
gibo update
```
{% endraw %}