---
layout: default
title: "reflex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reflex">
  <a href="/en/common/reflex.html">reflex</a> <a href="#reflex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to watch a directory and rerun a command when certain files change.
> More information: <https://github.com/cespare/reflex>.

#### Rebuild with `make` if any file changes:
```shell
reflex make
```
#### Compile and run Go application if any `.go` file changes:
```shell
reflex --regex='{{\.go$}}' {{go run .}}
```
#### Ignore a directory when watching for changes:
```shell
reflex --inverse-regex='{{^dir/}}' {{command}}
```
#### Run command when reflex starts and restarts on file changes:
```shell
reflex --start-service=true {{command}}
```
#### Substitute the filename that changed in:
```shell
reflex -- echo {}
```
{% endraw %}