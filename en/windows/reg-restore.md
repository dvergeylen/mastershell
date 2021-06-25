---
layout: default
title: "reg restore"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-restore">
  <a href="/en/windows/reg-restore.html">reg restore</a> <a href="#reg-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore a key and its values from a backup file.
> See `reg-save` for more information.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-restore>.

#### Overwrite a specified key with data from a backup file:
```shell
reg restore {{key_name}} {{path/to/file}}
```
{% endraw %}