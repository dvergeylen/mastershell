---
layout: default
title: "help2man"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="help2man">
  <a href="/en/common/help2man.html">help2man</a> <a href="#help2man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Produce simple man pages from an executable's `--help` and `--version` output.
> More information: <https://www.gnu.org/software/help2man>.

#### Generate a man page for an executable:
```shell
help2man {{executable}}
```
#### Specify the "name" paragraph in the man page:
```shell
help2man {{executable}} --name {{name}}
```
#### Specify the section for the man page (defaults to 1):
```shell
help2man {{executable}} --section {{section}}
```
#### Output to a file instead of stdout:
```shell
help2man {{executable}} --output {{path/to/file}}
```
#### Display detailed help:
```shell
help2man --help
```
{% endraw %}