---
layout: default
title: "doas"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doas">
  <a href="/en/common/doas.html">doas</a> <a href="#doas"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes a command as another user.
> More information: <https://man.openbsd.org/doas>.

#### Run a command as root:
```shell
doas {{command}}
```
#### Run a command as another user:
```shell
doas -u {{user}} {{command}}
```
#### Launch the default shell as root:
```shell
doas -s
```
#### Parse a config file and check if the execution of a command as another user is allowed:
```shell
doas -C {{config_file}} {{command}}
```
#### Make `doas` request a password even after it was supplied earlier:
```shell
doas -L
```
{% endraw %}