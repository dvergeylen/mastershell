---
layout: default
title: "forfiles"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="forfiles">
  <a href="/en/windows/forfiles.html">forfiles</a> <a href="#forfiles"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Select one or more files to execute a specified command on.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/forfiles>.

#### Search for files in the current directory:
```shell
forfiles
```
#### Search for files in a specific directory:
```shell
forfiles /p {{path/to/directory}}
```
#### Run the specified command for each file:
```shell
forfiles /c "{{command}}"
```
#### Search for files using a specific glob mask:
```shell
forfiles /m {{glob_pattern}}
```
#### Search for files recursively:
```shell
forfiles /s
```
#### Search for files older than 5 days:
```shell
forfiles /d {{+5}}
```
{% endraw %}