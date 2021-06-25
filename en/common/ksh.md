---
layout: default
title: "ksh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ksh">
  <a href="/en/common/ksh.html">ksh</a> <a href="#ksh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Korn Shell, a Bash-compatible command-line interpreter.
> See also `histexpand` for history expansion.
> More information: <http://kornshell.com>.

#### Start an interactive shell session:
```shell
ksh
```
#### Execute a command and then exit:
```shell
ksh -c "{{command}}"
```
#### Execute a script:
```shell
ksh {{path/to/script.ksh}}
```
#### Execute a script, printing each command before executing it:
```shell
ksh -x {{path/to/script.ksh}}
```
{% endraw %}