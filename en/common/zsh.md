---
layout: default
title: "zsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zsh">
  <a href="/en/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell, a Bash-compatible command-line interpreter.
> See also `histexpand` for history expansion.
> More information: <https://www.zsh.org>.

#### Start an interactive shell session:
```shell
zsh
```
#### Execute a command and then exit:
```shell
zsh -c "{{command}}"
```
#### Execute a script:
```shell
zsh {{path/to/script.zsh}}
```
#### Execute a script, printing each command before executing it:
```shell
zsh --xtrace {{path/to/script.zsh}}
```
#### Start an interactive shell session in verbose mode, printing each command before executing it:
```shell
zsh --verbose
```
{% endraw %}