---
layout: default
title: "go build"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-build">
  <a href="/en/common/go-build.html">go build</a> <a href="#go-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile Go sources.
> More information: <https://golang.org/cmd/go/#hdr-Compile_packages_and_dependencies>.

#### Compile a file:
```shell
go build {{path/to/main.go}}
```
#### Compile, specifying the output filename:
```shell
go build -o {{path/to/binary}} {{path/to/source.go}}
```
#### Compile a package:
```shell
go build -o {{path/to/binary}} {{path/to/package}}
```
#### Compile a main package into an executable, with data race detection:
```shell
go build -race -o {{path/to/executable}} {{path/to/main/package}}
```
{% endraw %}