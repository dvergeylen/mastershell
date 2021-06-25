---
layout: default
title: "dot_clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dot_clean">
  <a href="/en/osx/dot_clean.html">dot_clean</a> <a href="#dot_clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge ._* files with corresponding native files.
> More information: <https://ss64.com/osx/dot_clean.html>.

#### Merge all `._*` files recursively:
```shell
dot_clean {{path/to/directory}}
```
#### Don't recursively merge all `._*` in a directory (flat merge):
```shell
dot_clean -f {{path/to/directory}}
```
#### Merge and delete all `._*` files:
```shell
dot_clean -m {{path/to/directory}}
```
#### Only delete `._*` files if there's a matching native file:
```shell
dot_clean -n {{path/to/directory}}
```
#### Follow symlinks:
```shell
dot_clean -s {{path/to/directory}}
```
#### Print verbose output:
```shell
dot_clean -v {{path/to/directory}}
```
{% endraw %}