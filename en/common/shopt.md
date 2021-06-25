---
layout: default
title: "shopt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shopt">
  <a href="/en/common/shopt.html">shopt</a> <a href="#shopt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Bash shell options: variables (stored in `$BASHOPTS`) that control behavior specific to the Bash shell.
> Generic POSIX shell variables (stored in `$SHELLOPTS`) are managed with the `set` command instead.

#### List of all settable options and whether they are set:
```shell
shopt
```
#### Set an option:
```shell
shopt -s {{option_name}}
```
#### Unset an option:
```shell
shopt -u {{option_name}}
```
#### Print a list of all options and their status formatted as runnable `shopt` commands:
```shell
shopt -p
```
#### Show help for the command:
```shell
help shopt
```
{% endraw %}