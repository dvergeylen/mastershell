---
layout: default
title: "goimports"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="goimports">
  <a href="/en/common/goimports.html">goimports</a> <a href="#goimports"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Updates Go import lines, adding missing ones and removing unreferenced ones.
> More information: <https://godoc.org/golang.org/x/tools/cmd/goimports>.

#### Display the completed import source file:
```shell
goimports {{file}}.go
```
#### Write the result back to the source file instead of the standard output:
```shell
goimports -w {{file}}.go
```
#### Display diffs and write the result back to the source file:
```shell
goimports -w -d {{file}}.go
```
#### Set the import prefix string after 3rd-party packages (comma-separated list):
```shell
goimports -local {{path/to/package}} {{file}}.go
```
{% endraw %}