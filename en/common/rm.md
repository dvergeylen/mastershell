---
layout: default
title: "rm"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rm">
  <a href="/en/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove files or directories.
> More information: <https://www.gnu.org/software/coreutils/rm>.

#### Remove files from arbitrary locations:
```shell
rm {{path/to/file}} {{path/to/another/file}}
```
#### Recursively remove a directory and all its subdirectories:
```shell
rm -r {{path/to/directory}}
```
#### Forcibly remove a directory, without prompting for confirmation or showing error messages:
```shell
rm -rf {{path/to/directory}}
```
#### Interactively remove multiple files, with a prompt before every removal:
```shell
rm -i {{file(s)}}
```
#### Remove files in verbose mode, printing a message for each removed file:
```shell
rm -v {{path/to/directory/*}}
```
{% endraw %}