---
layout: default
title: "cmstp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cmstp">
  <a href="/en/windows/cmstp.html">cmstp</a> <a href="#cmstp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for managing connection service profiles.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/cmstp>.

#### Install a specific profile:
```shell
cmstp "{{path/to/profile}}"
```
#### Install without creating a desktop shortcut:
```shell
cmstp /ns "{{path/to/profile}}"
```
#### Install without checking for dependencies:
```shell
cmstp /nf "{{path/to/profile}}"
```
#### Only install for the current user:
```shell
cmstp /su "{{path/to/profile}}"
```
#### Install for all users (requires administrator privileges):
```shell
cmstp /au "{{path/to/profile}}"
```
#### Install silently without any prompts:
```shell
cmstp /s "{{path/to/profile}}"
```
#### Uninstall a specific profile:
```shell
cmstp /u "{{path/to/profile}}"
```
#### Uninstall silently without a confirmation prompt:
```shell
cmstp /u /s "{{path/to/profile}}"
```
{% endraw %}