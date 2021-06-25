---
layout: default
title: "doskey"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="doskey">
  <a href="/en/windows/doskey.html">doskey</a> <a href="#doskey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage macros, windows commands and command-lines.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/doskey>.

#### List available macros:
```shell
doskey /macros
```
#### Create a new macro:
```shell
doskey {{name}} = "{{command}}"
```
#### Create a new macro for a specific executable:
```shell
doskey /exename={{executable}} {{name}} = "{{command}}"
```
#### Remove a macro:
```shell
doskey {{name}} =
```
#### Display all commands that are stored in memory:
```shell
doskey /history
```
#### Save macros to a file for portability:
```shell
doskey /macros > {{macinit}}
```
#### Load macros from a file:
```shell
doskey /macrofile = {{macinit}}
```
{% endraw %}