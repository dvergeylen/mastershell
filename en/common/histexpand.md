---
layout: default
title: "history expansion"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="history-expansion">
  <a href="/en/common/histexpand.html">history expansion</a> <a href="#history-expansion"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reuse and expand the shell history in `sh`, `bash`, `zsh`, `rbash` and `ksh`.
> More information: <https://www.gnu.org/software/bash/manual/html_node/History-Interaction>.

#### Run the previous command:
```shell
!!
```
#### Run the previous command as root:
```shell
sudo !!
```
#### Run a command with the last argument of the previous command:
```shell
{{command}} !$
```
#### Run a command with the first argument of the previous command:
```shell
{{command}} !^
```
#### Run the command `n` lines back in the history:
```shell
!-{{n}}
```
#### Run the most recent command starting with `string`:
```shell
!{{string}}
```
#### Run the previous command, replacing `string1` with `string2`:
```shell
^{{string1}}^{{string2}}^
```
#### Perform a history expansion, but print the command that would be run instead of actually running it:
```shell
{{!-n}}:p
```
{% endraw %}