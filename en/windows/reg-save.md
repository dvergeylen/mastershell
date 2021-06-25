---
layout: default
title: "reg save"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-save">
  <a href="/en/windows/reg-save.html">reg save</a> <a href="#reg-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save a registry key, its sub keys and values to a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-save>.

#### Save a registry key, its sub keys and values to a specific file:
```shell
reg save {{key_name}} {{path/to/file}}
```
#### Forcefully overwrite an existing file without a prompt:
```shell
reg save {{key_name}} {{path/to/file}} /y
```
{% endraw %}