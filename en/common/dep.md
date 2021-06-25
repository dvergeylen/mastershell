---
layout: default
title: "dep"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dep">
  <a href="/en/common/dep.html">dep</a> <a href="#dep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool for deployment of PHP applications.
> Note: The Go command `dep` with the same name is deprecated and archived.
> More information: <https://deployer.org>.

#### Interactively initialize deployer in the local path (use a framework template with `--template={{template}}`):
```shell
dep init
```
#### Deploy an application to a remote host:
```shell
dep deploy {{hostname}}
```
#### Rollback to the previous working release:
```shell
dep rollback
```
#### Connect to a remote host via ssh:
```shell
dep ssh {{hostname}}
```
#### List commands:
```shell
dep list
```
#### Run any arbitrary command on the remote hosts:
```shell
dep run "{{command}}"
```
#### Display help for a command:
```shell
dep help {{command}}
```
{% endraw %}