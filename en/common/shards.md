---
layout: default
title: "shards"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shards">
  <a href="/en/common/shards.html">shards</a> <a href="#shards"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dependency management tool for the Crystal language.
> More information: <https://crystal-lang.org/reference/the_shards_command>.

#### Create a skeleton `shard.yml` file:
```shell
shards init
```
#### Install dependencies from a `shard.yml` file:
```shell
shards install
```
#### Update all dependencies:
```shell
shards update
```
#### List all installed dependencies:
```shell
shards list
```
#### List version of dependency:
```shell
shards version {{path/to/dependency_directory}}
```
{% endraw %}