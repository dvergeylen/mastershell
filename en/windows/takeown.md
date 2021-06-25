---
layout: default
title: "takeown"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="takeown">
  <a href="/en/windows/takeown.html">takeown</a> <a href="#takeown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Take ownership of a file or directory.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/takeown>.

#### Take ownership of the specified file:
```shell
takeown /f {{path/to/file}}
```
#### Take ownership of the specified directory:
```shell
takeown /d {{path/to/directory}}
```
#### Take ownership of the specified directory and all subdirectories:
```shell
takeown /r /d {{path/to/directory}}
```
#### Change ownership to the Administrator group instead of the current user:
```shell
takeown /a /f {{path/to/file}}
```
{% endraw %}