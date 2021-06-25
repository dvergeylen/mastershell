---
layout: default
title: "fc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fc">
  <a href="/en/windows/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare the differences between two files or sets of files.
> Use wildcards (*) to compare sets of files.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/fc>.

#### Compare 2 specified files:
```shell
fc {{path/to/file_1}} {{path/to/file_2}}
```
#### Perform a case-insensitive comparison:
```shell
fc /c {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as Unicode text:
```shell
fc /u {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as ASCII text:
```shell
fc /l {{path/to/file_1}} {{path/to/file_2}}
```
#### Compare files as binary:
```shell
fc /b {{path/to/file_1}} {{path/to/file_2}}
```
#### Disable tab-to-space expansion:
```shell
fc /t {{path/to/file_1}} {{path/to/file_2}}
```
#### Compress whitespace (tabs and spaces) for comparisons:
```shell
fc /w {{path/to/file_1}} {{path/to/file_2}}
```
{% endraw %}