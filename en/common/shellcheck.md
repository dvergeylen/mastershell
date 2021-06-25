---
layout: default
title: "shellcheck"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="shellcheck">
  <a href="/en/common/shellcheck.html">shellcheck</a> <a href="#shellcheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shell script static analysis tool.
> Check shell scripts for errors, usage of deprecated/insecure features, and bad practices.
> More information: <https://www.shellcheck.net>.

#### Check a shell script:
```shell
shellcheck {{path/to/script.sh}}
```
#### Check a shell script interpreting it as the specified shell dialect (overrides the shebang at the top of the script):
```shell
shellcheck --shell {{sh|bash|dash|ksh}} {{path/to/script.sh}}
```
#### Ignore one or more error types:
```shell
shellcheck --exclude {{SC1009,SC1073}} {{path/to/script.sh}}
```
#### Also check any sourced shell scripts:
```shell
shellcheck --checked-sourced {{path/to/script.sh}}
```
#### Display output in the specified format (defaults to `tty`):
```shell
shellcheck --format {{tty|checkstyle|diff|gcc|json|json1|quiet}} {{path/to/script.sh}}
```
#### Enable one or more optional checks:
```shell
shellcheck --enable={{add-default-case|avoid-nullary-conditions}}
```
#### List all available optional checks that are disabled by default:
```shell
shellcheck --list-optional
```
{% endraw %}