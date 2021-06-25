---
layout: default
title: "reg load"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-load">
  <a href="/en/windows/reg-load.html">reg load</a> <a href="#reg-load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Load saved sub keys into a different sub key in the registry.
> This is intended for troubleshooting and temporary keys.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-load>.

#### Load a backup file into the specified key:
```shell
reg load {{key_name}} {{path/to/file}}
```
{% endraw %}