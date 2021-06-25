---
layout: default
title: "reg unload"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-unload">
  <a href="/en/windows/reg-unload.html">reg unload</a> <a href="#reg-unload"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove data from the registry that was loaded using the `reg load` command.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-unload>.

#### Remove data from the registry for a specified key:
```shell
reg unload {{key_name}}
```
{% endraw %}