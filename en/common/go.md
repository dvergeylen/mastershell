---
layout: default
title: "go"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go">
  <a href="/en/common/go.html">go</a> <a href="#go"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing go source code.
> More information: <https://golang.org>.

#### Download and install a package, specified by its import path:
```shell
go get {{package_path}}
```
#### Compile and run a source file (it has to contain a `main` package):
```shell
go run {{file}}.go
```
#### Compile a source file into a named executable:
```shell
go build -o {{executable}} {{file}}.go
```
#### Compile the package present in the current directory:
```shell
go build
```
#### Execute all test cases of the current package (files have to end with `_test.go`):
```shell
go test
```
#### Compile and install the current package:
```shell
go install
```
#### Initialize a new module in the current directory:
```shell
go mod init {{module_name}}
```
{% endraw %}