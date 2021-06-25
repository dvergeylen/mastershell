---
layout: default
title: "crystal"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crystal">
  <a href="/en/common/crystal.html">crystal</a> <a href="#crystal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing Crystal source code.
> More information: <https://crystal-lang.org/reference/using_the_compiler>.

#### Run a Crystal file:
```shell
crystal {{path/to/file.cr}}
```
#### Compile a file and all dependencies to a single executable:
```shell
crystal build {{path/to/file.cr}}
```
#### Start a local interactive server for testing the language:
```shell
crystal play
```
#### Create a project directory for a Crystal application:
```shell
crystal init app {{application_name}}
```
#### Display all help options:
```shell
crystal help
```
{% endraw %}