---
layout: default
title: "go clean"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-clean">
  <a href="/en/common/go-clean.html">go clean</a> <a href="#go-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove object files and cached files.
> More information: <https://golang.org/cmd/go/#hdr-Remove_object_files_and_cached_files>.

#### Print the remove commands instead of actually removing anything:
```shell
go clean -n
```
#### Delete the build cache:
```shell
go clean -cache
```
#### Delete all cached test results:
```shell
go clean -testcache
```
#### Delete the module cache:
```shell
go clean -modcache
```
{% endraw %}