---
layout: default
title: "export"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="export">
  <a href="/en/linux/export.html">export</a> <a href="#export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command to mark shell variables in the current environment to be exported with any newly forked child processes.

#### Set a new environment variable:
```shell
export {{VARIABLE}}={{value}}
```
#### Remove an environment variable:
```shell
export -n {{VARIABLE}}
```
#### Mark a shell function for export:
```shell
export -f {{FUNCTION_NAME}}
```
#### Append something to the PATH variable:
```shell
export PATH=$PATH:{{path/to/append}}
```
{% endraw %}