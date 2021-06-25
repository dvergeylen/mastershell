---
layout: default
title: "go list"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-list">
  <a href="/en/common/go-list.html">go list</a> <a href="#go-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List packages or modules.
> More information: <https://golang.org/cmd/go/#hdr-List_packages_or_modules>.

#### List packages:
```shell
go list ./...
```
#### List standard packages:
```shell
go list std
```
#### List packages in json format:
```shell
go list -json time net/http
```
#### List module dependencies and available updates:
```shell
go list -m -u all
```
{% endraw %}