---
layout: default
title: "xonsh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xonsh">
  <a href="/en/common/xonsh.html">xonsh</a> <a href="#xonsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python-powered, cross-platform, Unix-gazing shell.
> Write and mix sh/Python code in Xonsh (pronounced conch).
> More information: <https://xon.sh>.

#### Start an interactive shell session:
```shell
xonsh
```
#### Execute a single command and then exit:
```shell
xonsh -c "{{command}}"
```
#### Run commands from a script file and then exit:
```shell
xonsh {{path/to/script_file.xonsh}}
```
#### Define environment variables for the shell process:
```shell
xonsh -D{{name1}}={{value1}} -D{{name2}}={{value2}}
```
#### Load the specified `.xonsh` or `.json` configuration files:
```shell
xonsh --rc {{path/to/file1.xonsh}} {{path/to/file2.json}}
```
#### Skip loading the `.xonshrc` configuration file:
```shell
xonsh --no-rc
```
{% endraw %}