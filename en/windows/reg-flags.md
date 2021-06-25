---
layout: default
title: "reg flags"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="reg-flags">
  <a href="/en/windows/reg-flags.html">reg flags</a> <a href="#reg-flags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display or set flags on registry keys.
> More information: <https://docs.microsoft.com/windows-server/administration/windows-commands/reg-flags>.

#### Display current flags for a specific key:
```shell
reg flags {{key_name}} query
```
#### Display help and available flag types:
```shell
reg flags /?
```
#### Set specified space-separated flags, and unset unmentioned flags, for a specific key:
```shell
reg flags {{key_name}} set {{flag_names}}
```
#### Set specified flags for a specific key and its sub keys:
```shell
reg flags {{key_name}} set {{flag_names}} /s
```
{% endraw %}