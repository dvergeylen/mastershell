---
layout: default
title: "fish"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fish">
  <a href="/en/common/fish.html">fish</a> <a href="#fish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Friendly Interactive SHell, a command-line interpreter designed to be user friendly.
> More information: <https://fishshell.com>.

#### Start an interactive shell session:
```shell
fish
```
#### Execute a command and then exit:
```shell
fish -c "{{command}}"
```
#### Execute a script:
```shell
fish {{path/to/script.fish}}
```
#### Check a script for syntax errors:
```shell
fish --no-execute {{path/to/script.fish}}
```
#### Start an interactive shell session in private mode, where the shell does not access old history or save new history:
```shell
fish --private
```
#### Display version information and exit:
```shell
fish --version
```
#### Set and export environmental variables that persist across shell restarts (from within the shell only):
```shell
set -Ux {{variable_name}} {{variable_value}}
```
{% endraw %}