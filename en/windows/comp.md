---
layout: default
title: "comp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="comp">
  <a href="/en/windows/comp.html">comp</a> <a href="#comp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare the contents of two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/comp>.

#### Compare files interactively:
```shell
comp
```
#### Compare two specified files:
```shell
comp {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare two sets of files:
```shell
comp {{path/to/directory_1/*}} {{path/to/directory_2/*}}
```
#### Display differences in decimal format:
```shell
comp /d {{path/to/file_1}} {{path/to/file_2}}
```
#### Display differences in ASCII format:
```shell
comp /a {{path/to/file_1}} {{path/to/file_2}}
```
#### Display line numbers for differences:
```shell
comp /l {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files case-insensitively:
```shell
comp /c {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare only the first 5 lines of each file:
```shell
comp /n={{5}} {{path/to/file_1}} {{path/to/file_2}}
```
{% endraw %}