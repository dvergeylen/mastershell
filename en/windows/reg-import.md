---
layout: default
title: "reg import"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-import">
  <a href="/en/windows/reg-import.html">reg import</a> <a href="#reg-import"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Import all available keys, subkeys, and values from a file.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-import>.

#### Import all keys, subkeys and values from a file:
```shell
reg import {{path/to/file.reg}}
```
{% endraw %}