---
layout: default
title: "set"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="set">
  <a href="/en/windows/set.html">set</a> <a href="#set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set environment variables for the current instance of CMD.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/set>.

#### List all current environment variables:
```shell
set
```
#### Set an environment variable to a specific value:
```shell
set {{name}}={{value}}
```
#### List environment variables starting with the specified string:
```shell
set {{name}}
```
#### Prompt the user for a value for the specified variable:
```shell
set /p {{name}}={{prompt_string}}
```
{% endraw %}