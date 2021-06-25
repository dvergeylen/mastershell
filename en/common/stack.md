---
layout: default
title: "stack"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="stack">
  <a href="/en/common/stack.html">stack</a> <a href="#stack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing Haskell projects.
> More information: <https://github.com/commercialhaskell/stack>.

#### Create a new package:
```shell
stack new {{package_name}} {{template_name}}
```
#### Compile a package:
```shell
stack build
```
#### Run tests inside a package:
```shell
stack test
```
#### Compile a project and re-compile every time a file changes:
```shell
stack build --file-watch
```
#### Compile a project and execute a command after compilation:
```shell
stack build --exec "{{command}}"
```
#### Run a program and pass an argument to it:
```shell
stack exec {{program_name}} -- {{argument}}
```
{% endraw %}