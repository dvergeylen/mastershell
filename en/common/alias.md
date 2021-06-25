---
layout: default
title: "alias"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="alias">
  <a href="/en/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates aliases -- words that are replaced by a command string.
> Aliases expire with the current shell session unless defined in the shell's configuration file, e.g. `~/.bashrc`.
> More information: <https://tldp.org/LDP/abs/html/aliases.html>.

#### List all aliases:
```shell
alias
```
#### Create a generic alias:
```shell
alias {{word}}="{{command}}"
```
#### View the command associated to a given alias:
```shell
alias {{word}}
```
#### Remove an aliased command:
```shell
unalias {{word}}
```
#### Turn `rm` into an interactive command:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Create `la` as a shortcut for `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}