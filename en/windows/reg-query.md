---
layout: default
title: "reg query"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-query">
  <a href="/en/windows/reg-query.html">reg query</a> <a href="#reg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the values of keys and sub keys in the registry.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-query>.

#### Display all values of a key:
```shell
reg query {{key_name}}
```
#### Display a specific value of a key:
```shell
reg query {{key_name}} /v {{value}}
```
#### Display all values of a key and its sub keys:
```shell
reg query {{key_name}} /s
```
#### Search for keys and values matching a specific pattern:
```shell
reg query {{key_name}} /f "{{query_pattern}}"
```
#### Display a value of a key matching a specified data type:
```shell
reg query {{key_name}} /t {{type}}
```
{% endraw %}