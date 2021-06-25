---
layout: default
title: "dash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dash">
  <a href="/en/common/dash.html">dash</a> <a href="#dash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian Almquist Shell, a modern, POSIX-compliant implementation of `sh` (not Bash-compatible).
> More information: <https://manned.org/dash>.

#### Start an interactive shell session:
```shell
dash
```
#### Execute a command and then exit:
```shell
dash -c "{{command}}"
```
#### Execute a script:
```shell
dash {{path/to/script.sh}}
```
#### Run commands from a script, printing each command before executing it:
```shell
dash -x {{path/to/script.sh}}
```
#### Execute commands from a script, stopping at the first error:
```shell
dash -e {{path/to/script.sh}}
```
#### Read and execute commands from stdin:
```shell
dash -s
```
{% endraw %}