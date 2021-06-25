---
layout: default
title: "wsl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="wsl">
  <a href="/en/windows/wsl.html">wsl</a> <a href="#wsl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the Windows Subsystem for Linux from the command-line.
> More information: <https://docs.microsoft.com/windows/wsl/reference>.

#### Start a Linux shell (in the default distribution):
```shell
wsl {{shell_command}}
```
#### Run a Linux command without using a shell:
```shell
wsl --exec {{command}} {{command_arguments}}
```
#### Specify a particular distribution:
```shell
wsl --distribution {{distribution}} {{shell_command}}
```
#### List available distributions:
```shell
wsl --list
```
#### Export a distribution to a `.tar` file:
```shell
wsl --export {{distribution}} {{path/to/distro_fs.tar}}
```
#### Import a distribution from a `.tar` file:
```shell
wsl --import {{distribution}} {{path/to/install_location}} {{path/to/distro_fs.tar}}
```
#### Change the version of the specified distribution:
```shell
wsl --set-version {{distribution}} {{version}}
```
#### Shut down Windows Subsystem for Linux:
```shell
wsl --shutdown
```
{% endraw %}