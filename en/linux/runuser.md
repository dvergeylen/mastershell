---
layout: default
title: "runuser"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="runuser">
  <a href="/en/linux/runuser.html">runuser</a> <a href="#runuser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run commands as a specific user and group without asking for password (needs root privileges).

#### Run command as a different user:
```shell
runuser {{user}} -c '{{command}}'
```
#### Run command as a different user and group:
```shell
runuser {{user}} -g {{group}} -c '{{command}}'
```
#### Start a login shell as a specific user:
```shell
runuser {{user}} -l
```
#### Specify a shell for running instead of the default shell (also works for login):
```shell
runuser {{user}} -s {{/bin/sh}}
```
#### Preserve the entire environment of root (only if `--login` is not specified):
```shell
runuser {{user}} --preserve-environment -c '{{command}}'
```
{% endraw %}