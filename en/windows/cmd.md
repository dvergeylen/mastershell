---
layout: default
title: "cmd"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmd">
  <a href="/en/windows/cmd.html">cmd</a> <a href="#cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Windows command interpreter.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmd>.

#### Start a new instance of the command interpreter:
```shell
cmd
```
#### Run the specified command and then exit:
```shell
cmd /c "{{command}}"
```
#### Run the specified command and then enter an interactive shell:
```shell
cmd /k "{{command}}"
```
#### Disable the usage of `echo` in command output:
```shell
cmd /q
```
#### Enable or disable command extensions:
```shell
cmd /e:{{on|off}}
```
#### Enable or disable file or directory autocompletion:
```shell
cmd /f:{{on|off}}
```
#### Enable or disable environment variable expansion:
```shell
cmd /v:{{on|off}}
```
#### Force output to use Unicode encoding:
```shell
cmd /u
```
{% endraw %}