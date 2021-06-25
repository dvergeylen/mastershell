---
layout: default
title: "rubocop"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rubocop">
  <a href="/en/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lint Ruby files.

#### Check all files in the current directory (including subdirectories):
```shell
rubocop
```
#### Check one or more specific files or directories:
```shell
rubocop {{path/to/file}} {{path/to/directory}}
```
#### Write output to file:
```shell
rubocop --out {{path/to/file}}
```
#### View list of cops (linter rules):
```shell
rubocop --show-cops
```
#### Exclude a cop:
```shell
rubocop --except {{cop_1}} {{cop_2}}
```
#### Run only specified cops:
```shell
rubocop --only {{cop_1}} {{cop_2}}
```
#### Auto-correct files (experimental):
```shell
rubocop --auto-correct
```
{% endraw %}