---
layout: default
title: "rector"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rector">
  <a href="/en/common/rector.html">rector</a> <a href="#rector"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An automated tool for updating and refactoring PHP 5.3+ code.
> More information: <https://github.com/rectorphp/rector>.

#### Process a specific directory:
```shell
rector process {{path/to/directory}}
```
#### Process a directory without applying changes (dry run):
```shell
rector process {{path/to/directory}} --dry-run
```
#### Process a directory and apply coding standards:
```shell
rector process {{path/to/directory}} --with-style
```
#### Display a list of available levels:
```shell
rector levels
```
#### Process a directory with a specific level:
```shell
rector process {{path/to/directory}} --level {{level_name}}
```
{% endraw %}