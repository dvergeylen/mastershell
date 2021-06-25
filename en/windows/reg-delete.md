---
layout: default
title: "reg delete"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-delete">
  <a href="/en/windows/reg-delete.html">reg delete</a> <a href="#reg-delete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete keys or their values from the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-delete>.

#### Delete a specific registry key:
```shell
reg delete {{key_name}}
```
#### Delete a value under a specific key:
```shell
reg delete {{key_name}} /v {{value}}
```
#### Delete all values recursively under the specified key:
```shell
reg delete {{key_name}} /va
```
#### Forcefully delete all values recursively under a key without a prompt:
```shell
reg delete {{key_name}} /f /va
```
{% endraw %}