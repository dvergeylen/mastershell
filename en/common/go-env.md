---
layout: default
title: "go env"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="go-env">
  <a href="/en/common/go-env.html">go env</a> <a href="#go-env"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage environment variables used by the Go toolchain.
> More information: <https://golang.org/cmd/go/#hdr-Print_Go_environment_information>.

#### Show all environment variables:
```shell
go env
```
#### Show a specific environment variable:
```shell
go env {{GOPATH}}
```
#### Set an environment variable to a value:
```shell
go env -w {{GOBIN}}={{path/to/directory}}
```
#### Reset an environment variable's value:
```shell
go env -u {{GOBIN}}
```
{% endraw %}