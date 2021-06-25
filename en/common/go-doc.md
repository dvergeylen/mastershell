---
layout: default
title: "go doc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-doc">
  <a href="/en/common/go-doc.html">go doc</a> <a href="#go-doc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show documentation for a package or symbol.
> More information: <https://golang.org/cmd/go/#hdr-Show_documentation_for_package_or_symbol>.

#### Show documentation for the current package:
```shell
go doc
```
#### Show package documentation and exported symbols:
```shell
go doc {{encoding/json}}
```
#### Show also documentation of symbols:
```shell
go doc -all {{encoding/json}}
```
#### Show also sources:
```shell
go doc -all -src {{encoding/json}}
```
#### Show a specific symbol:
```shell
go doc -all -src {{encoding/json.Number}}
```
{% endraw %}