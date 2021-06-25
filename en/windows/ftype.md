---
layout: default
title: "ftype"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ftype">
  <a href="/en/windows/ftype.html">ftype</a> <a href="#ftype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or modify file types used for file extension association.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/ftype>.

#### Display a list of all file types:
```shell
ftype
```
#### Display the associated program for a specific file type:
```shell
ftype {{file_type}}
```
#### Set the associated program for a specific file type:
```shell
ftype {{file_type}}="{{path/to/executable_command}}"
```
{% endraw %}