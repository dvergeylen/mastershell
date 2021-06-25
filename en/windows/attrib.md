---
layout: default
title: "attrib"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="attrib">
  <a href="/en/windows/attrib.html">attrib</a> <a href="#attrib"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays or changes file and directory attributes.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/attrib>.

#### Display the attributes of the files in the current directory:
```shell
attrib
```
#### Display the attributes of the files in the current directory and sub-directories:
```shell
attrib /S
```
#### Display the attributes of the files and directories in the current directory and sub-directories:
```shell
attrib /S /D
```
#### Add the read-only attribute to a file:
```shell
attrib +R {{document.txt}}
```
#### Remove the system and hidden attributes of a file:
```shell
attrib -S -H {{document.txt}}
```
#### Add the hidden attribute to a directory:
```shell
attrib +H {{path\to\directory}}
```
{% endraw %}