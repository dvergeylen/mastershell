---
layout: default
title: "go test"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-test">
  <a href="/en/common/go-test.html">go test</a> <a href="#go-test"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tests Go packages (files have to end with `_test.go`).
> More information: <https://golang.org/cmd/go/#hdr-Testing_flags>.

#### Test the package found in the current directory:
```shell
go test
```
#### [v]erbosely test the package in the current directory:
```shell
go test -v
```
#### Test the packages in the current directory and all subdirectories (note the `...`):
```shell
go test -v ./...
```
#### Test the package in the current directory and run all benchmarks:
```shell
go test -v -bench .
```
#### Test the package in the current directory and run all benchmarks for 50 seconds:
```shell
go test -v -bench . -benchtime {{50s}}
```
{% endraw %}