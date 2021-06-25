---
layout: default
title: "dex"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dex">
  <a href="/en/linux/dex.html">dex</a> <a href="#dex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DesktopEntry Execution is a program to generate and execute DesktopEntry files of the Application type.
> More information: <https://github.com/jceb/dex>.

#### Execute all programs in the autostart folders:
```shell
dex --autostart
```
#### Execute all programs in the specified folders:
```shell
dex --autostart --search-paths {{path/to/directory1}}:{{path/to/directory2}}:{{path/to/directory3}}:
```
#### Preview the programs would be executed in a GNOME specific autostart:
```shell
dex --autostart --environment {{GNOME}}
```
#### Preview the programs would be executed in a regular autostart:
```shell
dex --autostart --dry-run
```
#### Preview the value of the DesktopEntry property `Name`:
```shell
dex --property {{Name}} {{path/to/file.desktop}}
```
#### Create a DesktopEntry for a program in the current directory:
```shell
dex --create {{path/to/file.desktop}}
```
#### Execute a single program (with `Terminal=true` in the desktop file) in the given terminal:
```shell
dex --term {{terminal}} {{path/to/file.desktop}}
```
{% endraw %}