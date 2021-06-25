---
layout: default
title: "starship"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="starship">
  <a href="/en/common/starship.html">starship</a> <a href="#starship"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The minimal, blazing-fast, and infinitely customizable prompt for any shell.
> More information: <https://starship.rs>.

#### Print the starship integration code for the specified shell:
```shell
starship init {{bash|elvish|fish|ion|powershell|tcsh|zsh}}
```
#### Explain each part of the current prompt and show the time taken to render them:
```shell
starship explain
```
#### Print the computed starship configuration (use `--default` to print default configuration instead):
```shell
starship print-config
```
#### List supported modules:
```shell
starship module --list
```
#### Edit the starship configuration in the default editor:
```shell
starship configure
```
#### Create a bug report GitHub issue pre-populated with information about the system and starship configuration:
```shell
starship bug-report
```
#### Print the completion script for the specified shell:
```shell
starship completions {{bash|elvish|fish|powershell|zsh}}
```
#### Display help for a subcommand:
```shell
starship {{subcommand}} --help
```
{% endraw %}