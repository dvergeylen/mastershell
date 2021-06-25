---
layout: default
title: "reg copy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-copy">
  <a href="/en/windows/reg-copy.html">reg copy</a> <a href="#reg-copy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy keys and their values in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-copy>.

#### Copy a registry key to a new registry location:
```shell
reg copy {{old_key_name}} {{new_key_name}}
```
#### Copy a registry key recursively to a new registry location:
```shell
reg copy {{old_key_name}} {{new_key_name}} /s
```
#### Forcefully copy a registry key without a prompt:
```shell
reg copy {{old_key_name}} {{new_key_name}} /f
```
{% endraw %}