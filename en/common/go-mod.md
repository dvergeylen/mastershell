---
layout: default
title: "go mod"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-mod">
  <a href="/en/common/go-mod.html">go mod</a> <a href="#go-mod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Module maintenance.
> More information: <https://golang.org/cmd/go/#hdr-Module_maintenance>.

#### Initialize new module in current directory:
```shell
go mod init {{moduleName}}
```
#### Download modules to local cache:
```shell
go mod download
```
#### Add missing and remove unused modules:
```shell
go mod tidy
```
#### Verify dependencies have expected content:
```shell
go mod verify
```
#### Copy sources of all dependencies into the vendor directory:
```shell
go mod vendor
```
{% endraw %}