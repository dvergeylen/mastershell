---
layout: default
title: "reg export"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-export">
  <a href="/en/windows/reg-export.html">reg export</a> <a href="#reg-export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Export the specified sub keys and values into a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-export>.

#### Export all sub keys and values of a specific key:
```shell
reg export {{key_name}} {{path/to/file.reg}}
```
#### Force overwriting of an existing file without prompt:
```shell
reg export {{key_name}} {{path/to/file.reg}} /y
```
{% endraw %}