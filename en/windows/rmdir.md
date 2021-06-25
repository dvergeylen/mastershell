---
layout: default
title: "rmdir"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rmdir">
  <a href="/en/windows/rmdir.html">rmdir</a> <a href="#rmdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a directory and its contents.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/rmdir>.

#### Remove an empty directory:
```shell
rmdir {{path/to/directory}}
```
#### Remove a directory and its contents recursively:
```shell
rmdir {{path/to/directory}} /s
```
#### Remove a directory and its contents recursively without prompting:
```shell
rmdir {{path/to/directory}} /s /q
```
{% endraw %}