---
layout: default
title: "reg add"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-add">
  <a href="/en/windows/reg-add.html">reg add</a> <a href="#reg-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add new keys and their values to the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-add>.

#### Add a new registry key:
```shell
reg add {{key_name}}
```
#### Add a new value under a specific key:
```shell
reg add {{key_name}} /v {{value}}
```
#### Add a new value with specific data:
```shell
reg add {{key_name}} /d {{data}}
```
#### Add a new value to a key with a specific data type:
```shell
reg add {{key_name}} /t {{type}}
```
#### Forcefully overwrite the existing registry value without a prompt:
```shell
reg add {{key_name}} /f
```
{% endraw %}